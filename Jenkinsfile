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
        
        stage ('Initialize') {
            steps {
               sh '''
                    echo "PATH = ${PATH}"
                   echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }

       
    }
}
