pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation .. Creating a zip file'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/gradletest.zip'
            }
        }

    }
}
