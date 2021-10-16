pipeline {
    agent any
     tools {
  gradle 'Gradle'
}
   stages {
       stage('Build the Dockerfile') {
           steps {
             bat 'gradle build'
           }
       }
         stage('Build docker file'){
            steps {
              bat 'gradle docker'    
        }
     }
        stage('Run the Dockerfile') {
            steps {
                bat 'gradle dockerRun'
            }
        }
       
    }
}
