pipeline {
    // We’ll choose an agent per stage
    agent none

    stages {
        stage('service1') {
            agent { label 'Built-In Node' }       // controller
            steps {
                echo 'Hello World1 this is jenkins'
                bat 'cd'                          // show current directory
                bat 'dir'                         // list files
            }
        }

        stage('service2') {
            agent { label 'server_node_101' }     // your Windows server node
            steps {
                echo 'Hello World2 jenkins2'
                bat 'cd'                          // show current directory
                bat 'dir'
            }
        }

        stage('service3') {
            agent any
            steps {
                echo 'just HI from Built in'
            }
        }
    }
}
