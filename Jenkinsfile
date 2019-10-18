pipeline {
    agent any
    tools { 
        maven 'MAVEN_HOME' 
        jdk 'JAVA_HOME' 
    }
    stages {
        
         stage ('Build') {
            steps {
                echo 'This is a minimal pipeline.'
            }
        }
        
        
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
