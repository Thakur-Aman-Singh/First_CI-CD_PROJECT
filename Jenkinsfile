pipeline{

    agent any
  
  stages{

    stage("compiling"){

      steps{

        sh 'javac User.java'
        sh 'javac Student.java'
        sh 'javac FirstDemo.java'

      }
    }

    stage("running"){

     steps{
    
    sh 'java FirstDemo.java'

    
     }
    
    }

  }
 
  post{

   
   always{

     sh 'echo always running'
      
   }

   success{

   sh 'echo success build'

   }

   failure{

    sh 'echo build failure'
   }


  }


}