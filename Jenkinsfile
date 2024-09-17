pipeline {
    agent any

    stages {
        stage("Verify branch") {
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stage('Docker Build') {
            steps {
                sh 'docker-compose build'
                
            }
        }
        stage('Start App'){
            steps{
                sh 'docker-compose up -d'
            }
        }
    }

}