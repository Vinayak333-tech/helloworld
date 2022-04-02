pipeline{
  agent any  
  environment {
    NEW_VERSION = '0.1.0'
  }
  stages{
       stage("build"){
         when {
           expression {
              BRANCH_NAME == 'main'
           }
         }
         steps{
           echo "building version ${NEW_VERSION}"
           echo 'building version ${NEW_VERSION}'
         }
       }
        stage("test"){
         steps{ 
           echo "testing the aplication"
         }
       }
        stage("deploy"){
         steps{
           echo "deploying the aplication"
         }
       }
  }

}
