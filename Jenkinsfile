pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp0 -Dsonar.organization=asgbuggywebapp0 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2092b4b94057f41064b37b0661da65331fbabb2b'
			}
        } 
  }
}
