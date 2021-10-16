pipeline {
    agent any
  stages {
      stage ('checkout scm'){
          steps {
            sh 'checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-cred', url: 'https://github.com/udaybukke1/Impact-Petclinic.git']]]'
          }
      }
        stage('Build docker file'){
            steps {
              sh 'gradle docker'    
        }
     }
        stage('Run the Dockerfile') {
            steps {
                sh 'gradle dockerRun'
            }
        }
    }
}
