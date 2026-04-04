pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/YashAdhau9211/my-app.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
