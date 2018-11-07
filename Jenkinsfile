pipeline {
    agent any

    stages {
        stage('testStage') {
            steps {
                echo 'It is alive..'
                sh "docker build -v /var/run/docker.sock:/var/run/docker.sock -t test-image ."

            }
        }
    }
}
