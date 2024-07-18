pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                withMaven(maven : 'maven') {
                    sh 'mvn clean install'
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