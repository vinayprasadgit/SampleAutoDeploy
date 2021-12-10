pipeline {
    agent any
    environment{
        PATH="/opt/maven/bin:$PATH"
    }
    stages {
        stage('Test') {
            steps {
<<<<<<< HEAD
               sh 'mvn test'
            }
        }
        stage('Build Code') {
            steps {
                sh "mvn clean install"
=======
                sh "mvn clean test"
            }
        }
        stage('git checkout') {
            steps {
               git branch: 'feature2', url: 'https://github.com/vinayprasadgit/SampleAutoDeploy.git'
>>>>>>> ba8ef334bf010f8e83aab33d81bda1589f420e52
            }
        }
    }
}
