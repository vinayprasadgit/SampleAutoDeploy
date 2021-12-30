pipeline {
    agent any
    environment{
        PATH="/opt/maven/bin:$PATH"
    }
    stages {
        stage('Test') {
            steps {
               sh 'mvn test'
            }
        }
        stage('Build Code') {
            steps {
                sh "mvn clean install"
            }
        }
    }
}
