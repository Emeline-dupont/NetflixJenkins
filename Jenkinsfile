pipeline {
    agent any
    tools{
        jdk 'JDK8'
        maven 'Maven3'
         }

    stages {
        stage ('Initialize') {
            steps {
                bat '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
                }

            }
        }
    }
