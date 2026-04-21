pipeline {
    agent any

    

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Naveen04jan/ven.git'
            }
        }
        stages {
        stage('Build') {
            steps {
                sh 'mvn -v'
                sh 'java -version'
                sh 'mvn clean install'
            }
        }
    }

        stage('Build') {
            steps {
                sh 'mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
