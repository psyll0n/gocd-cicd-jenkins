
pipeline {
    agent any
    stages {
        stage("Pulling GoCD Image from Docker Hub...") { 
             steps {  
                sh "docker pull gocd/gocd-server:v21.1.0"
            }
        }
        stage("Running GoCD Server in Docker.") { 
            steps {  
                sh "docker run -d --name gocd-server -p8153:8153 -p8154:8154 gocd/gocd-server:v21.1.0"
            }
        }
    }
}
