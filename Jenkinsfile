pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'gcc+ -o PES1UG20CS685_file PES1UG20CS685_file.cpp'
                echo 'Build Stage Successful'
            }
        }

        stage('Test') {
            steps {
                sh './PES1UG20CS685_file'
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
                echo 'Pipeline Failed'
            }
        }
}
