pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }

        
    stage('Deploy') {
            steps {
                echo 'Hello Deploy'
                sh "whoami"
                sh "pwd"
                sh "ls -lrt"
                sh "kubectl apply -f ./demo-go.yaml"
            }
        }
        
    stage('Check Pod') {
            steps {
                echo 'Hello Check pod'
                sh "whoami"
                sh "pwd"
                sh "kubectl get pod -n demo-go-ns"
            }
        }
        
    }
    

        

    
}
