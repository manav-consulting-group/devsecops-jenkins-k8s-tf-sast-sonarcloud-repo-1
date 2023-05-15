pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vandyckbuggywebapp -Dsonar.organization=vandyckbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=686e875d7ddd878c8dbd758797f209b9f5f2575f'
			}
        } 
  }
}
