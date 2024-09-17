@Library('https://github.com/Ammar478/demo-shared-pipeline')

pipeline{
    agent any
    stages{
        stage('Call Library function with an argument'){
            steps{
                script {
                    helloWorld()
                }
            }
        }
    }
}