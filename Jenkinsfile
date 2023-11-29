pipeline {
    agent any
    tools {nodejs 'node'}

    
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('install Jest'){
            npm install --save-dev --g jest-cli
        }
        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
            
        }
    }

    post {
        always {
            // Clean up, notify, or perform any other post-build actions
          echo 'googTown'
        }
    }
}
