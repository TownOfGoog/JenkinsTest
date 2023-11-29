tpipeline {
    agent any
    tools {nodejs 'node'}

    
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        
        stage('Install jest') {
            steps {
                sh 'npm install jest-cli --g'
            }
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
