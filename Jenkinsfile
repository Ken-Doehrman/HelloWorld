pipeline {
    agent any 
    stages {
        stage('Clean') { 
            steps {
		sh "rm -f HelloWorld.sh"
            }
        }
        stage('Build') { 
            steps {
		sh "./HelloWorldBuild.sh"
            }
        }
        stage('Run') { 
            steps {
                sh "pwd"
                sh "ls -l"
                sh "./HelloWorld.sh"
            }
        }
    }
}
