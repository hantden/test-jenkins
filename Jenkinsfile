pipeline {
    agent any

    stages {
        stage('testStage') {
            steps {
                echo 'It is alive..'
                 def customImage = docker.build("my-image:${env.BUILD_ID}")
                 customImage.inside {
                  sh 'make test'
                 }
            }
        }
    }
}
