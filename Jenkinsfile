pipeline {
    agent any

    stages {
        stage('testStage') {
            steps {
                echo 'It is alive..'
                sh "docker build  -t test-image ."

            }
        }
    }
}
