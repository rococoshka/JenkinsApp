pipeline {
    agent { docker { image 'python:latest'}}

    environment {
        PROJECT_NAME = "govnoproject"
        OWNER_NAME = "rococo"
    }

    
    stages {
        stage('First stage') {
            steps {
                echo 'Hello from Jenkins'
            }
        }    
        stage('Second stage') {
            steps {
                echo 'Hello from Jenkins again'
                sh '''
                    echo "Command from shell"
                    ls -la
                    uname -a
                '''
                    echo "Poject: ${PROJECT_NAME}"
            }
        }    
        stage('Third stage') {
            steps {
                echo 'Hello from Jenkins again and again'
                echo "My name is ${OWNER_NAME}"
            }            
        }
    }
}
