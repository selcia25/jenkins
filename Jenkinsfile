pipeline {
    agent any

    stages {
        stage("Checkout") {
            steps {
                git branch: "main", url: "https://github.com/selcia25/jenkins.git"
            }
        }
        stage("Compile") {
            steps {
                sh "javac sample.java"
            }
        }
        stage("Run") {
            steps {
                sh "java sample"
            }
        }
        
    }
}
