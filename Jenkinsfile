pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappkan -Dsonar.organization=asgbuggywebappkan -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=45032e5433422334694a725682faf916c686e22a'
			}
        } 
  }
}
