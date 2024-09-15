pipeline {
    agent any

    stages {
        state("Verify branch") {
            steps {
                echo "$GIT_BRANCH"
            }
        }
        stages ('Docker Build') {
            steps {
                sh(script:'docker compose build')
            }
        }
    }

}