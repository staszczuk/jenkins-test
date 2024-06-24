/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'python:3.12.4-alpine3.20' } }
    environment {
        http_proxy = 'http://proxy-dmz.intel.com:912'
        https_proxy = 'http://proxy-dmz.intel.com:912'
        no_proxy = 'localhost,127.0.0.1,.intel.com'
    }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
