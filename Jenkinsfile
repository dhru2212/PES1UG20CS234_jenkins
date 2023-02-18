pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG20CS234-1', wait: false
                 echo 'Success -M B Dhruva'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Testing -M B Dhruva'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Success -M B Dhruva'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
