pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    docker_image = docker.build("${env.DOCKER_IMAGE_TAG}", '-f ./Dockerfile .')
                }
            }
        }
}
