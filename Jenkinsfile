pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                withMaven(maven: 'maven3'){
                    sh "mvn clean verify -DskipTests"
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}