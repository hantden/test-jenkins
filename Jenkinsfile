pipeline {
    agent any

    stages {
        stage('testStage') {
            steps {
                echo 'It is alive..'
                sh "docker build  -t ${env.REGISTRY_HOST}/library/test-image ."
                sh "docker push ${env.REGISTRY_HOST}/library/test-image"

            }
        }
    }
}
