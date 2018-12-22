pipeline {
    agent any
        stages {
                stage('Ansible') {
                        steps {
				ansiblePlaybook(
					installation: 'ansible-2.5',
					playbook: 'playbook.yml',
					colorized: true,
				)
                        }
                }
        }
}

