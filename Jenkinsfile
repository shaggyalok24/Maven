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
          sh "ls -lat"
         
          }
      }
     stage('deploy')
     {
      steps {
        
       echo "deploy"
        
        
       }
      }
   }
}
