pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=bobomanme -Dsonar.organization=bobomanme -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=ea9932f4c1857028d065b5727e409ee73785adf6'
			}
        } 
  }
}
