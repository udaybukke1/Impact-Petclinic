pipeline {
    agent any
      stages {
    stage('Checkout code') {
        steps {
            checkout scm
        }
    }
        stage('Build') {
            steps {
                sh 'gradle assemble'
            }
        }
        stage('Build1'){
            steps {
              sh 'gradle build'
            }
            
        }
        stage('Test') {
            steps {
                sh 'gradle test'
            }
        }
    }
}
