pipeline {
    anent any

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
            post {
                echo 'Now Archiving...'
                archiveArtifacts artifacts: '**/target/*.war'
            }
        }

     /*   stage('Deploy to Staging') {
            steps {

            }
        } */
    }
}