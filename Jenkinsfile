pipeline {    #prebuild
    agent any

    stages {      # build
        stage('Build') {
            steps {
                sh 'echo This is Build'
            }
        }

        stage('Test') {
            steps {
                sh 'echo This is test'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo This is deploy'
            }
        }
    }
}


post {    #post build
    always {
        echo "This section runs always"
    }

    success {
        echo "This section run when pipeline success"
    }

    failure {
        echo "This section run when pipeline failure"
    }
}