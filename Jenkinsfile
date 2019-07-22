pipeline {
    agent any 
    stages {
        stage('clean') { 
            steps {
    
                sh "mvn clean -f my-app"
            }
        }
        stage('Test') { 
            steps {
                   sh "mvn test -f my-app"
            }
        }
        stage('Deploy') { 
            steps {
                   sh "mvn package -f my-app"
            }
        }
    }
}
