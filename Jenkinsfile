pipeline {
    agent any

    environment {
        NAME = 'Jenkins'
        LASTNAME = 'Application'
    }

    stages {
         stage('Build') {
            withMaven(maven : 'maven') {
                sh 'mvn clean install'
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