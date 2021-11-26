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
        stage('git checkout') {
            steps {
               git branch: 'feature2', url: 'https://github.com/vinayprasadgit/SampleAutoDeploy.git'
            }
        }
    }
}
