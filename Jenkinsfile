pipeline {
    agent any
        stages {
                stage('Ansible') {
                        steps {
				ansiblePlaybook(
					installation: 'ansible_virtenv',
					playbook: 'playbook.yml',
					colorized: true,
				)
                        }
                }
        }
}

