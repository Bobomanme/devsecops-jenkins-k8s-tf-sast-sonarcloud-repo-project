pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp -Dsonar.organization=asgbuggywebappkey -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=2ec377df6c46e72d216ba0bb6fe98a20c5b6cff8'
			}
        } 
  }
}
