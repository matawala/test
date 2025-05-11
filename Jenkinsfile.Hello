pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'master', url: 'https://github.com/matawala/test.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                ansiblePlaybook playbook: 'playbook.yml'
            }
        }
    }
}
