pipeline{

    agent any
  
  stages{

    stage("compile"){

      steps{

        sh 'javac User.java'
        sh 'javac Student.java'
        sh 'javac FirstDemo.java'

      }
    }

    stage("run"){

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