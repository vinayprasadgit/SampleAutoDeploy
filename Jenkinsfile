pipeline {
    agent any
    environment{
        PATH="/opt/maven/bin:$PATH"
    }
    stages {
        stage('Test') {
            when {
                expression {
                    BRANCH_NAME =='feature3'
                }
            }
            steps {
                sh "mvn clean test"
                echo "Testing Completed for ${BRANCH_NAME}"
            }
        }
    }
}
