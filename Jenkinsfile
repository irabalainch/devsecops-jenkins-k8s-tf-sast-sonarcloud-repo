pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=aebuggytest -Dsonar.organization=aebuggytest -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f8275b8d18c54d0403cd5771b87782e674cc8742'
			}
        } 
  }
}
