pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                echo 'No tests available yet'
            }
        }

        stage('Run API') {
            steps {
                sh 'nohup npm start &'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished.'
        }
    }
}
