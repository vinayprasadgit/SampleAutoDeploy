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
        stage('git checkout') {
            steps {
               git branch: 'feature3', url: 'https://github.com/vinayprasadgit/SampleAutoDeploy.git'
            }
        }
    }
}
