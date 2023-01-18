pipeline {
  agent any
  
  stages {
     stage('chekout')
       {
         steps {
            echo "build"
            }
        }
     stage('test')
     {
       steps {
         
          echo "test"
         
          }
      }
     stage('deploy')
     {
      steps {
        
       echo "deploy"
       sh "ls -lat"
        
       }
      }
   }
}
