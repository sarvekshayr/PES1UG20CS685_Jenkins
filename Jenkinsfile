pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS685-1 PES1UG20CS685-1.cpp'
            }
        }

        stage('Test') {
            steps {
                sh './PES1UG20CS685-1'
            }
        }

        stage('Deploy') {
            steps {
                echo 'deployed successfully'
            }
        }
    }

    post {
        failure {
           echo 'Pipeline failed'
        }
    }
}
