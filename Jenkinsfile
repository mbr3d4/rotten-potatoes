pipeline {
    agent any

    stages {
        stage ('Deploy Kubernetes'){
            steps {
                withKubeConfig([credentialsId: 'Kubernetes']) {
                    sh 'kubectl apply -f ./k8s/deployment.yaml'
                }
            }
        }
    }
}