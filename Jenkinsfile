pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=appsec1 -Dsonar.organization=appsec1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=554be4e9a539d69d4013bb8f7737b212775a0922'
			}
        } 
  }
}
