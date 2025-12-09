pipeline {
    agent none
    stages {
        stage('checkout') {
            agent { label 'built-in' }
            steps {
                git branch: 'main',
                    credentialsId: 'git_jenkins',
                    url: 'https://github.com/harshahchawan/OppsPillers'
            }
        }
    }
}
