pipeline {
    agent any
    stages {
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
