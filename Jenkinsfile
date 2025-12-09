pipeline {
    agent none

    stages {

        stage('checkout') {
            agent { label 'Built-In Node' }
            steps {
                git branch: 'main',
                    credentialsId: 'git_jenkins',
                    url: 'https://github.com/harshahchawan/Jenkins_pipeline'
            }
        }

        // stage('service2') {
        //     agent { label 'server_node_101' }
        //     steps {
        //         echo 'Hello World2 jenkins2'
        //         bat 'cd'
        //         bat 'dir'
        //     }
        // }

        // stage('service3') {
        //     agent any
        //     steps {
        //         echo 'just HI from Built in'
        //     }
        // }
    }
}
