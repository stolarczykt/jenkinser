pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo "Build number is ${currentBuild.number}"
                echo '==> Sleep 120 seconds'
                sleep 120
                echo '==> Woke up after 120 seconds'
            }
        }
    }
}
