
pipeline {
    agent any
    stages {
        stage("build") { 
             steps {  
                sh "docker pull gocd/gocd-server:v21.1.0"
            }
        }
        stage("run") { 
            steps {  
                sh "docker run -d --name gocd-server -p8153:8153 -p8154:8154 gocd/gocd-server:v21.1.0"
            }
        }
    }
}
