node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def mvn = tool 'Default Maven';
    withSonarQubeEnv() {
      sh "${mvn}/bin/mvn clean verify sonar:sonar -Dsonar.projectKey=Sindalah_Demo01182023"
    }
  }
  
 stage('Build') {
            steps {
                echo 'Building..'
		
				
            }
        }
 stage('Test') {
            steps {
                echo 'Testing..'
				
            }
        }
  stage('Deploy') {
            steps {
                echo 'Deploying....'
				
            }
        }
}
