pipeline {
    agent any   
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS685-1 my_cpp_file.cpp'
			          echo 'Build Stage Successful'
            }
        }
        
        stage('Test') {
            steps {
                sh './PES1UG20CS685-1'
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
        always {
            echo 'Pipeline completed'
        }
        
        failure {
            echo 'Pipeline failed'
        }
    }
}
