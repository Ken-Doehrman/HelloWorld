pipeline {
    agent any 
    stages {
        stage('Clean') { 
            steps {
		rm -f HelloWorld.sh
            }
        }
        stage('Build') { 
            steps {
		sh ./HelloWorldBuild.sh
            }
        }
        stage('Run') { 
            steps {
                sh ./HelloWorld.sh
            }
        }
    }
}
