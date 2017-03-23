pipeline {
    agent docker {python '2.7.10'}
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
