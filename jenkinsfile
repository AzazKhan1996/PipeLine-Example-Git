pipeline {
    agent any

    stages {
        stage("Compile") {
            steps {
                bat 'javac Student.java'
            }
        }

        stage("Run") {
            steps {
                bat 'java Student'
            }
        }
    }
}
