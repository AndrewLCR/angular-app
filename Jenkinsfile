pipeline {
    agent {
        label 'windows-worker'
    }

    stages {
        stage('Version verification') {
            when {
                branch 'prod'
            }
            steps {
                bat 'ng version'
            }

             when {
                branch 'dev'
            }
            steps {
                bat 'ng version'
            }
        }

        stage('Install dependencies') {
            when {
                branch 'prod'
            }
            steps {
                bat 'npm install'
            }

             when {
                branch 'dev'
            }
            steps {
                bat 'ng version'
            }
        }

        stage('Lint tests') {
            when {
                branch 'prod'
            }
            steps {
                bat 'ng lint'
            }

             when {
                branch 'dev'
            }
            steps {
                bat 'ng version'
            }
        }

        stage('Unit Tests') {
            when {
                branch 'prod'
            }
            steps {
                bat 'ng test'
            }

             when {
                branch 'dev'
            }
            steps {
                bat 'ng version'
            }
        }

        stage('Build application') {
            when {
                branch 'prod'
            }
            steps {
                bat 'ng build'
            }

             when {
                branch 'dev'
            }
            steps {
                bat 'ng version'
            }
        }
    }
}
