pipeline {
    agent any
    
    stages {
        
        stage('github-clone') {
            steps {
                git branch: 'main', credentialsId: 'github-test', url: '{REPOSITORY URL}'
            }
        }
        
   		// stage...
   	}
}
