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
      
      stage('SonarQube analysis') {
         withSonarQubeEnv('My SonarQube Server') {
         sh 'mvn clean package sonar:sonar'
         } // submitted SonarQube taskId is automatically attached to the pipeline context
      }     
      
   }
}
