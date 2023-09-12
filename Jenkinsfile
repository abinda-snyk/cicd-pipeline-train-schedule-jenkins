pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --gradle-version=7.2'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
