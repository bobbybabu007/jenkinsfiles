pipeline {
    agent any

    tools {
        maven 'M3'
    }

    stages {
        stage('SCM') {
            steps {
                sh 'Checkoing out 1-declarative branch'
                git branch: '1-declarative', url: 'https://github.com/bobbybabu007/jenkinsfiles.git'
            }
        }
    }
        stage('Build') {
            steps {
                sh 'mvn -B package'
            }
        }
    }
}
