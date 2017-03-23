pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                timeout(time: 3, units: 'MINUTES') {
                    retry(3) {
                        bat 'set'
                    }
                }
            }
        }
    }
}
