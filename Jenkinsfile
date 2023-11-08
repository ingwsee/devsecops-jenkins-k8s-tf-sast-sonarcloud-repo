pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebappfromasg -Dsonar.organization=buggywebappfromasg -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=67f2929906399be4799d82cdcaf230800ec9f821'
			}
        } 
  }
}
