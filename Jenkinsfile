pipeline {
    agent any
    tools { 
        maven 'MAVEN_HOME' 
        jdk 'jdk-12.0.1' 
    }
    stages {
        stage ('Initialize') {
            steps {
               sh '''
                    echo "PATH = ${PATH}"
                    echo "MAVEN_HOME = ${MAVEN_HOME}"
                '''
            }
        }

        stage ('Build') {
            steps {
                echo 'This is a minimal pipeline.'
            }
        }
    }
}
