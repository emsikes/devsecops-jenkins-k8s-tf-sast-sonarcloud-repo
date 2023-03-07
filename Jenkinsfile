pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=clouddevopsbuggywebapp -Dsonar.organization=clouddevopsbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login='1284c9333cfbc99ffe6855a7e0cabaff9ded13bd'
			}
        } 
  }
}
