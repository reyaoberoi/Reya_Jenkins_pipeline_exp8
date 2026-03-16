pipeline {
    agent any

    stages {

        stage('Clean Old Directories') {
            steps {
                bat '''
                IF EXIST C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Reya_Pipeline_exp8\\JOB_1 (
                    rmdir /s /q C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Reya_Pipeline_exp8\\JOB_1
                )
                '''
                echo 'Old folders deleted if they existed'
            }
        }

        stage('Create JOB_1') {
            steps {
                bat 'mkdir C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Reya_Pipeline_exp8\\JOB_1'
                echo 'JOB_1 created'
            }
        }

        stage('Create JOB_2') {
            steps {
                bat 'mkdir C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Reya_Pipeline_exp8\\JOB_1\\JOB_2'
                echo 'JOB_2 created inside JOB_1'
            }
        }

        stage('Create JOB_3') {
            steps {
                bat 'mkdir C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Reya_Pipeline_exp8\\JOB_1\\JOB_2\\JOB_3'
                echo 'JOB_3 created inside JOB_2'
            }
        }

    }

    post {
        success {
            echo 'Directory structure created successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
