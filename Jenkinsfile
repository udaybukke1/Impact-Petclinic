pipeline {
    agent any
     tools {
  gradle 'Gradle'
}
   stages {
       stage('Build the Dockerfile') {
           steps {
             sh 'gradle build'
           }
       }
      /*   stage('Build docker file'){
            steps {
              sh 'gradle docker'    
        }
     }
        stage('Run the Dockerfile') {
            steps {
                sh 'gradle dockerRun'
            }
        }*/
       
    }
}
