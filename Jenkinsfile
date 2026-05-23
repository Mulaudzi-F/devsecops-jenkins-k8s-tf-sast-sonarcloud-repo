pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_8'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=fhatudevsec -Dsonar.organization=fhatudevsec -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1f6db6453ad3b89bf93c484c259392489b92fe3a'
			}
        } 
  }
}
