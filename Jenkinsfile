pipeline {
    agent any

    stages {
        stages("Verify branch") {
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