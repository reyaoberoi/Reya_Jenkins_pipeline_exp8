pipeline {
    agent any

    stages {

        stage('Delete Old Folder') {
            steps {
                bat '''
                IF EXIST C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Task2_Pipeline\\JOB_1 (
                    rmdir /s /q C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Task2_Pipeline\\JOB_1
                )
                '''
            }
        }

        stage('Create JOB_1') {
            steps {
                bat 'mkdir C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Task2_Pipeline\\JOB_1'
            }
        }

        stage('Create JOB_2') {
            steps {
                bat 'mkdir C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Task2_Pipeline\\JOB_1\\JOB_2'
            }
        }

        stage('Create JOB_3') {
            steps {
                bat 'mkdir C:\\ProgramData\\Jenkins\\.jenkins\\workspace\\Task2_Pipeline\\JOB_1\\JOB_2\\JOB_3'
            }
        }

    }
}
