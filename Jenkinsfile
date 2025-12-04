pipeline {
    agent none   // use per-stage agents

    stages {
        stage('service1') {
            agent { label 'Built-In Node' }   // label of your controller node
            steps {
                echo 'Hello World1 this is jenkins'
                bat 'echo %CD%'              // run on Built-In node
            }
        }

        stage('service2') {
            agent { label 'server_node_101' } // label of your new Windows server node
            steps {
                echo 'Hello World2 jenkins2'
                bat 'echo %CD%'              // runs on server_node_101
            }
        }

        stage('test') {
            agent any
            steps {
                echo 'Hello World3'
            }
        }
    }
}
