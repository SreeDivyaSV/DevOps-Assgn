pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('build') {
            steps {
                python main.py
            }
        }
        stage('test') {
            steps {
                python unit.py
            }
        }
    }
}
