pipeline {
    agent any
     tools {
  gradle 'Gradle'
}
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
