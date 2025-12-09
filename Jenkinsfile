pipeline {
    agent none
    stages {
        stage('checkout') {
            agent { label 'built-in' }
            steps {
                deleteDir()
                git credentialsId: 'git_jenkins',
                    url: 'https://github.com/harshahchawan/OppsPillers'
                bat 'dir'
                bat 'git branch -a'
            }
        }
    }
}
