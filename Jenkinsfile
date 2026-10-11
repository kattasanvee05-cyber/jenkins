pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application'
                bat 'if not exist index.html exit /b 1'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the application'
                bat 'findstr /C:"Hello from Jenkins CI" index.html'
            }
        }

        stage('Complete') {
            steps {
                echo 'Build and tests completed successfully'
            }
        }
    }
}
