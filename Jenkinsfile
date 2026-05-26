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
                // Change "sh" to "bat" for Windows!
                bat '"C:\apache-maven-3.9.11-bin\apache-maven-3.9.11\bin\mvn" clean package'
            }
        }
        stage('Test') {
            steps {
                // Change "sh" to "bat" for Windows!
                bat '"C:\apache-maven-3.9.11-bin\apache-maven-3.9.11\bin\mvn" test'
            }
        }
    }
}