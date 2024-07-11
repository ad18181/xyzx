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
                docker { image 'horuszup/horusec-cli:alpha' }
            } 
            steps {
                sh 'horusec start -p="./" --disable-docker="true" --config-file-path=horusec-config.json '
                sh'pwd'
            }
        }
        stage('st 3 ') {
            agent any 
            steps {
                sh '''
                pwd
                '''    
            }
           
        }

        

    }

}
