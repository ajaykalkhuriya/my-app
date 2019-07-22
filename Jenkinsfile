pipeline {
    agent any 
    stages {
        stage('clean') { 
            steps {
                 sh "git clone https://github.com/ajaykalkhuriya/my-app"  
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
