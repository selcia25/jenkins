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
                bat "javac sample.java"
            }
        }
        stage("Run") {
            steps {
                bat "java sample"
            }
        }
        
    }
}
