pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggy0 -Dsonar.organization=asgbuggy0 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2092b4b94057f41064b37b0661da65331fbabb2b'
			}
        } 
  }
}
