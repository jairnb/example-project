pipeline {
    agent any

    environment {
        NAME = 'Jenkins'
        LASTNAME = 'Application'
    }

    stages {
         stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}