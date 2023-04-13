pipeline {	
	agent any
	tools {
	maven 'Maven_3_5_2'
	}
	stages{
	stage('CompileandRunSonarAnalysis') {
	steps {
	sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=calobug -Dsonar.organization=calobug -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=47910261b9e4e1c98913e7ea1e9c77ddf3632bee'
	}
	}
	}
	}
