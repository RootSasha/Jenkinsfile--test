pipeline {
    agent any

    environment {
        DOCKER_HUB_REPO = 'sasha22mk/test-site'
        DOCKER_IMAGE_TAG = '2022-latest' // Або інший тег, який ви хочете пушити
    }

    stages {
        stage('Push Docker Image to Docker Hub') {
            steps {
                sh "docker push ${DOCKER_HUB_REPO}:${DOCKER_IMAGE_TAG}"
            }
        }
    }
}
