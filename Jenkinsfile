pipeline {
    agent any

    stages {

        stage('Create JOB_1 Directory') {
            steps {
                sh 'mkdir -p JOB_1'
                echo 'JOB_1 directory created'
            }
        }

        stage('Create JOB_2 Directory') {
            steps {
                sh 'mkdir -p JOB_1/JOB_2'
                echo 'JOB_2 directory created inside JOB_1'
            }
        }

        stage('Create JOB_3 Directory') {
            steps {
                sh 'mkdir -p JOB_1/JOB_2/JOB_3'
                echo 'JOB_3 directory created inside JOB_2'
            }
        }

    }
}
