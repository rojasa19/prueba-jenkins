pipeline {
    agent any
    tools {
        nodejs '16.11.1'
    }
    options {
        timeout(time: 2, unit: 'MINUTES')
    }
    stages {
        stage('Install dependencies') {
            steps {
                sh 'npm i'
            }
        }
        stage('Run tests') {
            steps {
                sh 'npm test'
            }
        }
    }
}