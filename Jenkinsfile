pipeline {
    agent any
        stages {
                stage('Ansible') {
                        steps {
                                ansiColor('xterm') {
                                        ansiblePlaybook(
                                                installation: 'ansible 2.4.3 (virtualenv)',
                                                playbook: 'main.yml',
                                                inventory: '/var/lib/jenkins/dynamic_inventory/foreman.py',
                                                limit: '${target}',
                                                credentialsId: 'jenkins_ssh_to_avtomat',
                                                colorized: true,
                                                sudoUser: 'avtomat',
                                                extras: '${dry_run}'
                                        )
                                }
                        }
                }
        }
}

