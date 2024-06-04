pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building the code...'
                    // Assuming the use of Maven as the build tool
                    echo 'Build Tool: Maven'
                }
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                script {
                    echo 'Running unit and integration tests...'
                    // Assuming the use of JUnit for unit tests and Selenium for integration tests
                    echo 'Test Tools: JUnit, Selenium'
                }
            }
        }

        stage('Code Analysis') {
            steps {
                script {
                    echo 'Performing code analysis...'
                    // Assuming the use of SonarQube for code analysis
                    echo 'Code Analysis Tool: SonarQube'
                }
            }
        }

        stage('Security Scan') {
            steps {
                script {
                    echo 'Performing security scan...'
                    // Assuming the use of OWASP Dependency-Check for security scanning
                    echo 'Security Scan Tool: OWASP Dependency-Check'
                }
            }
        }

        stage('Deploy to Staging') {
            steps {
                script {
                    echo 'Deploying to staging...'
                    // Assuming deployment to an AWS EC2 instance
                    echo 'Deployment Environment: AWS EC2'
                }
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                script {
                    echo 'Running integration tests on staging...'
                    // Assuming the use of Selenium for integration tests
                    echo 'Test Tools: Selenium'
                }
            }
        }

        stage('Deploy to Production') {
            steps {
                script {
                    echo 'Deploying to production...'
                    // Assuming deployment to an AWS EC2 instance
                    echo 'Deployment Environment: AWS EC2'
                }
            }
        }
    }

    post {
        always {
            emailext(
                to: 'kchandrakanth540@gmail.com',
                subject: "Pipeline Execution Result: ${currentBuild.currentResult}",
                body: "Pipeline execution ${currentBuild.currentResult}. Check the attached logs for more details.",
                attachLog: true,
                compressLog: true,
                recipientProviders: [[$class: 'DevelopersRecipientProvider']]
            )
        }
    }
}
