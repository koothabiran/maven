pipeline {
    agent any
    tools { 
        maven 'MAVEN_HOME' 
        jdk 'jdk-12.0.1' 
    }
    stages {
        
         stage ('Build') {
            steps {
                echo 'This is a minimal pipeline.'
            }
        }
        
        stage('Test') {
            steps {
                sh 'echo "Fail!"; exit 1'
            }
        }
    
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
        unstable {
            echo 'This will run only if the run was marked as unstable'
        }
        changed {
            echo 'This will run only if the state of the Pipeline has changed'
            echo 'For example, if the Pipeline was previously failing but is now successful'
        }
    }


       
    }
}
