pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               echo "Build is running" 
            }
        }
        stage('Test') {
            steps {
               configFileProvider([configFile(fileId: 'aniket.txt', targetLocation: '/var/jenkins_home/workspace/test', variable: 'ANI')]) {
    		// some block
		} 
            }
        }

	    stage('Deploy') {
            steps {
               echo "Deployment is done" 
            }
        }
    }
}        
