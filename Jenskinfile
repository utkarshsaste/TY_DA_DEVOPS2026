pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Build') {
            steps {
                echo 'No build needed for HTML'
            }
        }

        stage('Test') {
            steps {
                echo 'Checking if index.html exists'
                bat 'if exist index.html (echo File exists) else (exit 1)'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to XAMPP htdocs'
                bat 'copy index.html C:\\xampp\\htdocs\\'
            }
        }
    }
}

