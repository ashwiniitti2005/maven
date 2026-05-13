pipeline {
    agent any

    tools {
        maven 'Maven3'
        jdk 'JDK21'
    }

    stages {
      stage('checkout'){
        steps{
          git "

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
