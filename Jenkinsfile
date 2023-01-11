pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vikasdevbuggywebapp -Dsonar.organization=vikasdevbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1bb9f261b688b80bc95bbeca73b551c5f30b51ec'
			}
        } 
  }
}
