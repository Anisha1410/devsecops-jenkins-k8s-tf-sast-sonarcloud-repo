pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=webapp -Dsonar.organization=anisha-squiddytestapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=e56cf7994f54f5bc8ab6764f6e526d6f964e99ee'
			}
        } 
  }
}
