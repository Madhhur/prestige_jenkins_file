pipeline {
    agent { label 'worker7' }

    stages {
        stage('Hello from Worker') {
            steps {
                echo 'Hello! Running on worker node7.'
            }
        }

        stage('Check System Info') {
            steps {
                sh 'hostname'
                sh 'whoami'
                sh 'pwd'
                sh 'df -h'
            }
        }
    }

    post {
        always {
            echo 'Pipeline completed.'
           
        }
    }
}
