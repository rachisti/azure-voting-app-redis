pipeline {
   agent any

   stages {
      stage('Verify Branch') {
         steps {
            echo "$GIT_BRANCH"
         }
      }
      
      stage('build') {
         steps {
            echo "$JOB_NAME"
         }
      }      
      
      stage('Sonar analyze') {
         steps {
            echo "$JOB_NAME"
         }
      }         
      
   }
}
