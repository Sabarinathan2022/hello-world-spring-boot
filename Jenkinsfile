node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    withSonarQubeEnv() {
	    
      sh "./gradlew sonarqube"
    }
  }
  
 stage('Build') {
            steps {
		    	sh "mvn clean install"
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
