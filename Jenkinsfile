pipeline {
    any agent 
    stages {
        stage('Compile stage') {
            steps {
                withMaven(maven : 'maven-3.6.2')
                sh 'mvn clean compile'
            }
        }
    
      stage('Testing stage') {
            steps {
                withMaven(maven : 'maven-3.6.2')
                sh 'mvn clean test'
            }
        }
    
      stage('Deployment stage') {
            steps {
                withMaven(maven : 'maven-3.6.2')
                sh 'mvn deploy'
            }
        }
    }
}