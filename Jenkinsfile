pipeline {
    agent any

    stages {
        stage('github-clone') {
            steps {
                git branch: 'main', credentialsId: 'github-test', url: 'https://github.com/gnzmzn321/jenkins-test.git'
            }
        }

        stage('process-file') { // GitHub과 연동된 스테이지
            steps {
                script {
                    def filePath = 'README.md' // 처리할 파일 경로
                    if (fileExists(filePath)) {
                        echo "File '${filePath}' exists. Displaying content:"
                        echo readFile(filePath) // 파일 내용 출력
                    } else {
                        echo "File '${filePath}' does not exist."
                    }
                }
            }
        }
    }
}
