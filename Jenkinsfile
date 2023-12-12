pipeline {
    agent any
    environment {
        PATH = "/opt/maven3.9.6/bin:$PATH"
    }
    stages {
        stage("Git clone") {
            steps {
               git branch: "master", url: "https://github.com/nnsnarasimha/javamave.git"
            }
        }
        stage("Maven Build") {
            steps {
                sh "mvn clean install"
            }
        }
     }
 }

