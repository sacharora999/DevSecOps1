pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sachinorg -Dsonar.organization=sachinorg -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=319c98eea28b3bbdbb80a3a0f0a2c029f44e195e'
			}
        } 
  }
}
