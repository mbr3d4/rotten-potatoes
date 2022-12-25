pipeline {
    agent any

    stages {
        stage ('Deploy Kubernetes'){
            steps {
                withKubeConfig([credentialsId: 'Kubernetes']) {
                    sh 'kubectl delete -f ./k8s/deployment.yaml'
                }
            }
        }
    }
}