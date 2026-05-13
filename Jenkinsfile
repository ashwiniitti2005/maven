pipeline {
    agent any

    tools {
        maven 'maven3'
        jdk 'JDK21'
    }

    stages {

        stage('checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/ashwiniitti2005/maven.git'
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
