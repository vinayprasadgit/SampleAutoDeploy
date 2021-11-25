pipeline {
    agent any
    environment{
        PATH="/opt/maven/bin:$PATH"
    }
    stages {
        stage('Build Code') {
            steps {
                sh "mvn clean install"
            }
        }
    }
}
