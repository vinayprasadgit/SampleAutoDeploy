pipeline {
    agent any
    environment{
        PATH="/opt/maven/bin:$PATH"
    }
    stages {
        stage('git checkout') {
            steps {
               git branch: 'feature1', url: 'https://github.com/vinayprasadgit/SampleAutoDeploy.git'
            }
        }
    }
}
