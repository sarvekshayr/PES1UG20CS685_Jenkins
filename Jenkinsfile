pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o hello hello.cpp'
                echo 'PES1UG20CS685'
                echo 'Build Stage Successful'
            }
        }

        stage('Test') {
            steps {
                sh './hello'
                echo 'Test Stage Successful'
                
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy Stage Successful'
            }
        }
    }

    post {
        failure {
           echo 'Pipeline failed'
        }
    }
}
