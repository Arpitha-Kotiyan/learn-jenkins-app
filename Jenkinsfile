node {
    stage('Build') {
        docker.image('node:18-alpine').inside {
            sh '''
            ls -la
            node --version
            npm --version
            npm ci
            npm run build
            ls -la
            '''
        }
    }
}
