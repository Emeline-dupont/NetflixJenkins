pipeline {
    agent any
    tools{
        jdk 'jdk11'
        maven 'Maven3'
         }

    stages {

    stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
                }
            }

    stage('Run') {
            steps {
                sh returnStdout: true, script: 'java -jar  target/netflix-1.0.0.jar  netflix_titles.csv'

                }
            }
        }
    }

