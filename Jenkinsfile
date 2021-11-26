pipeline {
    agent any
    environment{
        PATH="/opt/maven/bin:$PATH"
    }
    stages {
        stage('Test') {
            steps {
                sh "mvn clean test"
            }
        }
        stages {
        stage('git checkout') {
            steps {
               git branch: 'master', url: 'https://github.com/vinayprasadgit/SampleAutoDeploy.git'
            }
        }
    }
}
