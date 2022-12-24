pipeline {
    agent any

    stages {
        stage ('Build Image') {
            steps {
                script {
                    dockerapp = docker.build("mbr3d4/rotten-potatoes", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}