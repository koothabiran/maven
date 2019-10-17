node{
    stage('SCM Checkout'){
        git 'https://github.com/koothabiran/maven.git'
    }
    stage('Compile-Package'){
        def mnvnHome = tool name: 'MAVEN_HOME', type: 'maven'
        sh "${mvnHome}/bin/mvn package"
            
    }
}
