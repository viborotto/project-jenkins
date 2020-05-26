pipeline {
    agent any 
    stages {
        stage('Prepare') { 
            steps {
                sh 'chmod a+x mvnw'
                sh './mvnw clean'
            }
        }
        stage('Compile') { 
            steps {
                sh './mvnw compile'
            }
        }
        stage('Build') { 
            steps {
                sh './mvnw -Dmaven.test.failure.ignore=true install'
            }
        }
        stage('Test') { 
            steps {
                //
            }
        }
        stage('Deploy') { 
            steps {
                //
            }
        }
    }
}
