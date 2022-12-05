#!groovy
pipeline {
    agent none
    stages {
        stage('Maven Install') {
            agent {
                docker {
                    image 'maven:3.5.0'
                    alwaysPull true
                }
            }
            steps {
                sh "ls"
                sh 'mvn clean install'
            }
        }
    }
}
