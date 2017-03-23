pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                timeout(time: 3, unit: 'MINUTES') {
                    retry(3) {
                        bat 'set'
                    }
                }
            }
        }
    }
    post {
        success {
            echo "Project build was successful."
        }
        failure {
            echo "Project build failed."
        }
    }
}
