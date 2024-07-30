pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo "Build number is ${currentBuild.number}"
                sh "git rev-parse HEAD > .git/current-commit"
                echo "==> Read from rev: ${readFile(".git/current-commit").trim()}"
                echo "==> Read from env: ${GIT_COMMIT}"
                echo '==> Sleep 120 seconds'
                sleep 120
                echo '==> Woke up after 120 seconds'
            }
        }
    }
}
