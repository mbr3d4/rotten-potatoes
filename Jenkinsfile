pipeline {
    agent any

    stages {
        stage ('Build Image') {
            steps {
                script {
                    dockerapp = docker.build("mbr3d4/rotten-potatoes:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}