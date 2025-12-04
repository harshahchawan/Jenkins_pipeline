pipeline {
    agent none

    stages {

        stage('service1') {
            agent { label 'built-in' }   // Fix label
            steps {
                echo 'Hello World1 this is jenkins'
                bat 'cd'
                bat 'dir'
            }
        }

        stage('service2') {
            agent { label 'server_node_101' }
            steps {
                echo 'Hello World2 jenkins2'
                bat 'cd'
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
