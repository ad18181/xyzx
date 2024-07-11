pipeline {

    agent any 

    stages {

        stage('Checkout') {

            steps {

                // Checkout code from the branch

                checkout scm

            }

        }
        
        stage('Build') {
            agent {
                docker { image 'busybox:latest' }
            } 
            steps {
                sh 'touch hello.txt'
            }
        }
        stage('st 3 ') {
            agent any 
            steps {
                sh 'ls'
            }
           
        }

        

    }

}
