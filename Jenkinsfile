pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Commands to build your project
                sh 'mvn clean package'
            }
        }
        
        stage('Test') {
            steps {
                // Commands to run tests
                sh 'mvn test'
            }
        }
        
        stage('Deploy') {
            steps {
                // Commands to deploy your application
                sh 'kubectl apply -f deployment.yaml'
            }
        }
    }
}
