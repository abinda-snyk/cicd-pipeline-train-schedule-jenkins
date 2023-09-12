pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon --warning-mode all'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
