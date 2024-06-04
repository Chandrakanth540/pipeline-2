pipeline {
  
  agent any
 
 
  stages {
   
    stage('Build Stage') {
      steps {
        echo 'Building the application...'
       
      }
      post {
        success {
          mail to: 'kchandrakanth540@gmail.com', 
          subject: 'Build Successful'
          body: 'The application build completed successfully.'
        }
        failure {
          mail to: 'kchandrakanth540@gmail.com', 
          subject: 'Build Failed'
          body: 'The application build encountered an error. Please review the Jenkins logs for details.'
        }
      }
    }
 

    stage('Test Stage') {
      steps {
        echo 'Running unit and integration tests...'
        
      }
      post {
        success {
          mail to: 'kchandrakanth540@gmail.com', 
          subject: 'Tests Passed'
          body: 'The application tests completed successfully.'
        }
        failure {
          mail to: 'kchandrakanth540@gmail.com',  
          subject: 'Tests Failed'
          body: 'The application tests encountered an error. Please review the Jenkins logs for details.'
        }
      }
    }
 
 
    stage('Code Analysis Stage') {
      steps {
        echo 'Performing code analysis...'
       
      }
      post {
        success {
          mail to: 'kchandrakanth540@gmail.com', 
          subject: 'Code Analysis Successful'
          body: 'The code analysis completed successfully.'
        }
        failure {
          mail to: 'kchandrakanth540@gmail.com',  
          subject: 'Code Analysis Failed'
          body: 'The code analysis encountered an error. Please review the Jenkins logs for details.'
        }
      }
    }

    stage('Security Scan Stage') {
      steps {
        echo 'Performing security scan...'
       
      }
      post {
        success {
          mail to: 'kchandrakanth540@gmail.com', 
          subject: 'Security Scan Successful'
          body: 'The security scan completed successfully.'
        }
        failure {
          mail to: 'kchandrakanth540@gmail.com',  
          subject: 'Security Scan Failed'
          functional  'The security scan encountered an error. Please review the Jenkins logs for details.'
        }
      }
    }
 
    stage('Deploy to Staging Environment') {
      steps {
        echo 'Deploying application to staging...'
      
      }
    }
 
    stage('Integration Tests on Staging') {
      steps {
        echo 'Executing integration tests in staging environment...'

      }
    }
 
    stage('Deploy to Production Environment') {
      steps {
        echo 'Deploying application to production...'

      }
    }
  }
}
