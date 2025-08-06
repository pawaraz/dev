pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Replace with your build command, e.g.,:
                // sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Replace with your test command, e.g.,:
                // sh 'npm test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Example: Docker build and run
                sh '''
                    docker build -t myapp .
                    docker run -d -p 80:80 myapp
                '''
            }
        }
    }
}
