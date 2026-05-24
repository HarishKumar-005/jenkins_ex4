pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/HarishKumar-005/jenkins_ex4.git'
            }
        }
        stage('Build') {
            steps {
                // Exact path to your Maven executable on Windows
                bat 'mvn" clean package'
            }
        }
        stage('Test') {
            steps {
                // Exact path for the testing process
                bat 'mvn" test'
            }
        }
    }
}