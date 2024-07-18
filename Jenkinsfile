pipeline {
    agent any

    environment {
        NAME = 'Jenkins'
        LASTNAME = 'Application'
    }

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven') {
                    sh 'mvn clean install'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven') {
                    sh 'mvn test'
                }
            }
        }


//         stage ('Deployment Stage') {
//             steps {
//                 withMaven(maven : 'maven') {
//                     sh 'mvn deploy'
//                 }
//             }
//         }
    }
}