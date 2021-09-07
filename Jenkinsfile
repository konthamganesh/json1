def envname = readJSON file: '${env.WORKSPACE}/manifest.json'
pipeline {
    agent any
    stages { 
        stage('Build') {
            steps {
                echo WORKSPACE
                sh "ls -a ${WORKSPACE}"
            } 
        }
        }
 }
