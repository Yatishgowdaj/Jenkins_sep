pipeline {

    agent {
        label 'machine-2'
    }

    stages {

        stage('Build') {
            steps {
                echo 'Starting Build...'

                sh '''
                    echo 'Building application...'
                    ls -la
                '''
            }
        }

        stage('Test') {
            steps {
                echo 'Starting Tests...'

                sh '''
                    echo "Running tests..."
                    echo "Tests completed successfully"
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Starting Deployment...'

                sh '''
                    echo "Deploying application..."
                    echo "Deployment completed successfully"
                '''
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}
