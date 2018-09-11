pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sleep 10
            }
        }
        stage('Test') {
            parallel {
                stage('API tests') {
                    steps {
                        echo 'Building..'
                        sleep 7
                    }
                }
                stage('Cypress tests') {
                    steps {
                        echo 'Building..'
                        sleep 8
                    }
                }
                stage('Protractor tests') {
                    steps {
                        echo 'Building..'
                        sleep 5
                    }
                }
                stage('Integration tests on Windows') {
                    steps {
                        echo 'Building..'
                        sleep 11
                    }
                }
                stage('Integration tests on Linux') {
                    steps {
                        echo 'Building..'
                        sleep 10
                    }
                }
            }
        }
        stage('Build documentation') {
            steps {
                echo 'Deploying....'
                sleep 2
            }
        }
        stage('Upload package') {
            steps {
                echo 'Deploying....'
                sleep 6
            }
        }
    }
}