/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'python:3.12.4-alpine3.20' } }
    environment {
        httpProxy = 'http://proxy-dmz.intel.com:912'
        httpsProxy = 'http://proxy-dmz.intel.com:912'
        noProxy = 'localhost,127.0.0.1,.intel.com'
    }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
