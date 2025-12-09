pipeline {
    agent none
    stages {
        stage('checkout') {
            agent { label 'built-in' }
            steps {
                // Delete everything in workspace first
                deleteDir()
                
                // Now clone OppsPillers
                git branch: 'main',
                    credentialsId: 'git_jenkins',
                    url: 'https://github.com/harshahchawan/OppsPillers'
                
                // Verify what's in workspace
                bat 'dir'
                bat 'git remote -v'
            }
        }
    }
}
