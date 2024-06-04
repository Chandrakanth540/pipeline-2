pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                    echo 'Building the code...'
                    // Assuming the use of Maven as the build tool
                    echo 'Build Tool: Maven'
            }
             post {
       success {
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline was successful', 
               body: 'successfully lauched pipeline' 
       } failure { 
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline Failure', 
               body: 'The pipeline encountered an error.' 
       } 
   }
        }
        

        stage('Unit and Integration Tests') {
            steps {
                    echo 'Running unit and integration tests...'
                    // Assuming the use of JUnit for unit tests and Selenium for integration tests
                    echo 'Test Tools: JUnit, Selenium'
                
            }
             post {
       success {
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline was successful', 
               body: 'successfully lauched pipeline' 
       } failure { 
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline Failure', 
               body: 'The pipeline encountered an error.' 
       } 
   }
        }

        stage('Code Analysis') {
            steps {
                    echo 'Performing code analysis...'
                    // Assuming the use of SonarQube for code analysis
                    echo 'Code Analysis Tool: SonarQube'
               
            }
             post {
       success {
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline was successful', 
               body: 'successfully lauched pipeline' 
       } failure { 
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline Failure', 
               body: 'The pipeline encountered an error.' 
       } 
   }
        }

        stage('Security Scan') {
            steps {
                    echo 'Performing security scan...'
                    // Assuming the use of OWASP Dependency-Check for security scanning
                    echo 'Security Scan Tool: OWASP Dependency-Check'
               
            }
             post {
       success {
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline was successful', 
               body: 'successfully lauched pipeline' 
       } failure { 
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline Failure', 
               body: 'The pipeline encountered an error.' 
       } 
   }
        }

        stage('Deploy to Staging') {
            steps {
                    echo 'Deploying to staging...'
                    // Assuming deployment to an AWS EC2 instance
                    echo 'Deployment Environment: AWS EC2'
               
            }
             post {
       success {
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline was successful', 
               body: 'successfully lauched pipeline' 
       } failure { 
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline Failure', 
               body: 'The pipeline encountered an error.' 
       } 
   }
        }

        stage('Integration Tests on Staging') {
            steps {
                    echo 'Running integration tests on staging...'
                    // Assuming the use of Selenium for integration tests
                    echo 'Test Tools: Selenium'
                
            }
             post {
       success {
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline was successful', 
               body: 'successfully lauched pipeline' 
       } failure { 
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline Failure', 
               body: 'The pipeline encountered an error.' 
       } 
   }
        }

        stage('Deploy to Production') {
            steps {
                    echo 'Deploying to production...'
                    // Assuming deployment to an AWS EC2 instance
                    echo 'Deployment Environment: AWS EC2'
               
            }
             post {
       success {
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline was successful', 
               body: 'successfully lauched pipeline' 
       } failure { 
           mail to: 'kchandrakanth540@gmail.com', 
               subject: 'Pipeline Failure', 
               body: 'The pipeline encountered an error.' 
       } 
   }
        }
    }

   
}
