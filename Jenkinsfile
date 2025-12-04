

pipeline {
    agent any

    stages {
        stage('service1') {
            steps {
                echo 'Hello World1 this is jenkins'
                sleep(time: 10, unit: 'SECONDS')
            }
        }
        stage('service2') {
            steps {
                echo 'Hello World2 jenkins2'
                sleep(time: 10, unit: 'SECONDS')
             
            }
        }
        stage('service3') {
            steps {
                echo 'Hello World3'
            }
        }
    }
}
