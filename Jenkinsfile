pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'GitHub code received'
            }
        }

        stage('Build') {
            steps {
                echo 'Building website...'
                sh 'ls -la'
            }
        }

        stage('Test') {
            steps {
                sh 'test -f index.html'
                echo 'Website test passed!'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Website ready for deployment!'
            }
        }
    }

    post {
        success {
            echo 'CI/CD Pipeline Successful!'
        }
    }
}