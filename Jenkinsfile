pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS240-1 try.cpp'
                pecho "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS240-1'
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS240-1'
            }
        }
    }
    post {
        always {
            pecho 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
