stage('Push SQL Image to Docker Hub') {
    steps {
        sh 'whoami'
        sh 'docker images | grep sasha22mk/test-site'
        sh 'docker info'
        sh 'sleep 10'
        sh '''
            docker push ${DOCKER_HUB_REPO}:2022-latest
        '''
    }
}
