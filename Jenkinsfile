pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bobomanme -Dsonar.organization=Bobomanme -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=d0f19cdb4b7c4a89848bc25b09336cd5ac915be4'
			}
        } 
  }
}
