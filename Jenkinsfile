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
        
         stages {
        stage ('Initialize') {
            steps {
                bat '''
                    echo "PATH = ${PATH}"
                    echo "MAVEN_HOME = ${MAVEN_HOME}"
                ''' 
            }
        }
   

       
    }
}
