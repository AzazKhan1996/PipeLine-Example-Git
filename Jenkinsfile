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

    post {
        success {
            echo "✅ Pipeline completed successfully!"
            bat 'echo Build and Run succeeded!'
        }
        failure {
            echo "❌ Pipeline failed!"
            bat 'echo Check errors in Build or Run stages.'
        }
        always {
            echo "🔹 This runs regardless of success or failure."
        }
    }
}
