pipeline {
    agent any
    
    stages {
        
        stage('github-clone') {
            steps {
                git branch: 'main', credentialsId: 'github_test', url: '{REPOSITORY URL}'
            }
        }
        
   		// stage...
   	}
}
