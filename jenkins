pipeline {
            agent any

            environment {
                PATH = "${env.PATH};C:\\Program Files\\nodejs\\"
                // replace "C:\\Program Files\\nodejs\\" with the actual path to the node js installation directory on your system
            }

            stages {
                stage('Install dependencies') {
                    steps {
                        bat 'npm install'
                    }
                }

                stage('Run tests') {
                    steps {
                        bat 'npm run test'
                    }
                }
            }
        }
