pipeline{
 agent any
  stages
  {
     stage("build")
    {
      steps{
      echo 'Building th eapplication'
       sh 'npm install npm'
      }
    }
    
    stage("test"){
      steps{
      echo 'Testing the application'
      }
    }
  
    stage("deploy")
    {
      steps{
      echo 'Deployinh the application'
      }
    
    }
    
    
  }
}
