pipeline {
    agent any
	tools{
		maven 'local-maven'
	}
    stages {
        stage('Build') {
            steps {
                bat label: '', script: 'mvn clean package'
            }
        }
        
    }
}