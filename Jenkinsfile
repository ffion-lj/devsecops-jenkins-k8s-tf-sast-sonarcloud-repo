pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=fasgbuggywebapp -Dsonar.organization=fasgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=43bd38940dcc45473d92b0a2a59b7bca31c1a146'
			}
        } 
  }
}
