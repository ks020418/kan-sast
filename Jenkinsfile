pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cwbuggyapp -Dsonar.organization=cwbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2de222c541fe21c2038265d5dc05291e9be836c3'
			}
        } 
  }
}
