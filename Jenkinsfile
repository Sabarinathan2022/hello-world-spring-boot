node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    withSonarQubeEnv() {
	    	mvn clean install
      sh "./gradlew sonarqube"
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
