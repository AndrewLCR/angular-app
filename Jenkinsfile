pipeline {
    agent {
        label 'windows-worker'
    }

    stages {
        stage('Version verification') {
            when {
                anyOf {
                    branch 'prod'
                    branch 'dev'
                }
            }
            steps {
                sh 'ng version'
            }
        }

        stage('Install dependencies') {
            when {
                anyOf {
                    branch 'prod'
                    branch 'dev'
                }
            }
            steps {
                sh 'ng version'
            }
        }

        stage('Lint tests') {
           when {
                anyOf {
                    branch 'prod'
                    branch 'dev'
                }
            }
            steps {
                sh 'ng version'
            }
        }

        stage('Unit Tests') {
           when {
                anyOf {
                    branch 'prod'
                    branch 'dev'
                }
            }
            steps {
                sh 'ng version'
            }
        }

        stage('Build application') {
            when {
                anyOf {
                    branch 'prod'
                    branch 'dev'
                }
            }
            steps {
                sh 'ng version'
            }
        }
    }
}
