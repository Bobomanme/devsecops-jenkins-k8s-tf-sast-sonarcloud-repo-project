pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggytoken -Dsonar.organization=asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=59e1e6768475cd3355fca24d6bdfb13ee6f661fa'
			}
        } 
  }
}
