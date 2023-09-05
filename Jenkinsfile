pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapps -Dsonar.organization=asgbuggywebapps -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=4b8388f216b0984a7c2c474ddd19bc49502d1fec'
			}
        } 
  }
}
