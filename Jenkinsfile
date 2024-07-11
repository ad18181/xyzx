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
                sh 'pwd'
            }
        }
        stage('st 3 ') {
            agent any 
            steps {
                sh 'pwd'
            }
           
        }

        

    }

}
