pipeline {
    agent any
	
    stages {
        stage('Build') {
            steps {
                bat script: 'mvn clean package'
            }
			post {
				success {
					echo 'archiving artifact...'
					archiveArtifact artifact:'**/*.war'
				}
			}
        }
        
    }
}