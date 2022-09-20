pipeline{
    options {
        timestamps()
    }
    agent any
    tools { 
        maven 'Maven 3.6.2' 
        jdk 'jdk8' 
    }
    stages{
        stage('checkout'){
            checkout scm
        }
        stage('build'){
            sh "mvn build"
        }
    }

}