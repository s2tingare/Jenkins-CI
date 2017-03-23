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
}
