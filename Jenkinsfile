pipeline {
    agent any
     tools {
  gradle 'Gradle'
}
   stages {
       stage('Compile the Source code') {
           steps {
             bat 'gradle build'
           }
       }
       stage('Test cases') {
           steps {
             bat 'gradle unit test'
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
