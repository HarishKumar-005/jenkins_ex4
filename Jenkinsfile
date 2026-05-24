pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clones your code automatically
                git branch: 'main', url: 'https://github.com/your-username/sample-app.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}