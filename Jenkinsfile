pipeline {
    agent any
    stages {
        stage('GradleW build') {
            steps {
                echo 'Running gradle build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
