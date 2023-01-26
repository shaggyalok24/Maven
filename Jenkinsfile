pipeline {
  agent any
  tools {
    maven 'maven'
  }
  environment {
        DATE = new Date().format('yy.M')
        TAG = "${DATE}.${BUILD_NUMBER}"
    }
    
  stages {
     stage('chekout')
       {
         steps {
            sh 'mvn clean package'
            }
        }
      
      stage('Docker Build') {
            steps {
                script {
                    docker.build("shggyalok24/hello-world:${TAG}")
                }
            }
        }
    
   
     stage('')
     {
      steps {
        
       echo "deploy"
       sh "ls -lat"
        
       }
      }
   }
}
