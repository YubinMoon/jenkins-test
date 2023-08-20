pipeline {
    agent { docker "python:3.10" }
    environment { 
        USERNAME = credentials("USERNAME")
        PASSWORD = credentials("PASSWORD")
    }
    stages {
        stage("run") {
            steps {
                echo 'run python'
                sh 'python hello.py $USERNAME $PASSWORD'
            }
        }
    }
}
