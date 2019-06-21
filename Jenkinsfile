pipeline {
    agent any
	
    stages {
        stage('Build') {
            steps {
                bat script: 'mvn clean package'
            }
			post {
				successs {
					echo 'archiving artifact...'
					archiveArtifact artifact: '**/*.war'
				}
			}
        }
        
    }
}