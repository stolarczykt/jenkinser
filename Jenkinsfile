pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo "Build number is ${currentBuild.number}"
                sh "git rev-parse HEAD > .git/current-commit"
                echo "==> Read from rev: ${readFile(".git/current-commit").trim()}"
                echo "==> GIT_COMMIT: ${GIT_COMMIT}"
                echo "==> GIT_PREVIOUS_COMMIT: ${GIT_PREVIOUS_COMMIT}"
                echo "==> GIT_PREVIOUS_SUCCESSFUL_COMMIT: ${GIT_PREVIOUS_SUCCESSFUL_COMMIT}"
                echo '==> Sleep 180 seconds'
                sleep 180
                echo '==> Woke up after 180 seconds'
            }
        }
    }
}
