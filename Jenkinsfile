pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/matawala/test.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                ansiblePlaybook playbook: 'playbook.yml'
            }
        }
    }
}
