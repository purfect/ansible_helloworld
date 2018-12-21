pipeline {
    agent any
        stages {
                stage('Ansible') {
                        steps {
                                        ansiblePlaybook(
                                                installation: 'ansible-2.5.0',
                                                playbook: 'main.yml',
                                                colorized: true,
                                        )
                        }
                }
        }
}

