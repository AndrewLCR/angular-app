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
                sh 'ng version'
            }

             when {
                branch 'dev'
            }
            steps {
                sh 'ng version'
            }
        }

        stage('Install dependencies') {
            when {
                branch 'prod'
            }
            steps {
                sh 'npm install'
            }

             when {
                branch 'dev'
            }
            steps {
                sh 'ng version'
            }
        }

        stage('Lint tests') {
            when {
                branch 'prod'
            }
            steps {
                sh 'ng lint'
            }

             when {
                branch 'dev'
            }
            steps {
                sh 'ng version'
            }
        }

        stage('Unit Tests') {
            when {
                branch 'prod'
            }
            steps {
                sh 'ng test'
            }

             when {
                branch 'dev'
            }
            steps {
                sh 'ng version'
            }
        }

        stage('Build application') {
            when {
                branch 'prod'
            }
            steps {
                sh 'ng build'
            }

             when {
                branch 'dev'
            }
            steps {
                sh 'ng version'
            }
        }
    }
}
