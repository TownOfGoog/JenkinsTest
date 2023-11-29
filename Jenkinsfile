pipeline {
    agent any
    tools {nodejs 'node'}

    
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
            
        }
        stage('install Jest'){
            npm install --save-dev jest
        }
    }

    post {
        always {
            // Clean up, notify, or perform any other post-build actions
          echo 'googTown'
        }
    }
}
