pipeline {
    agent any
    stages {
        stage('Github Checkout') {
            steps {
                git branch: 'main',
                    credentialsId: 'github_token',
                    url: 'https://github.com/NOOJU/ttest.git'
            }
        }
       
    }

    
    post {
        success {
            echo 'Playbook executed successfully!'
        }
        failure {
            echo 'Playbook execution failed!'
        }
    }
}     
