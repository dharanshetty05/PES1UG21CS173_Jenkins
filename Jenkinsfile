pipeline{
    agent any
    stages{  
      stage('Build') {
          steps {
            build 'PES1UG21CS173-1'    
            sh 'g++ ./main/test.cpp -o PES1UG21CS173-1'
          }
      }
          
      stage('Test') {
          steps {
            sh './PES1UG21CS173-123'
        }
    }
        
      stage('Deploy') {
          steps {
              echo 'Deploy'
          }
      }
    }

    post {
        failure {
            echo 'pipeline failed'
        }
    }
}
