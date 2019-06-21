pipeline {
    agent any
	tools{
		maven 'local-maven'
	}
    stages {
        stage('Build') {
            steps {
                bat script: 'mvn clean package'
            }
        }
        
    }
}