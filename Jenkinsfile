pipeline {
    agent any
    tools {
        maven 'maven'
    }
    stages {
        stage('Build the Jar file') {
            steps {
                sh 'mvn clean package'
            }
            post {
                success {
                    echo "success done with Build the Jar file"
                }
                failure {
                    echo "project failed with Build the Jar file"
                }
                always {
                    echo "am always will get execute from Build the Jar file"
                }
            }
        }
    }
    post {
        success {
            echo "success done with project"
        }
        failure {
            echo "project failed"
        }
        always {
            echo "am always will get execute"
        }
    }
}
