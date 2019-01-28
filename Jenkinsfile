#!/usr/bin/env groovy

@Library('piper-library-os-experimental') _

stage ('first stage') {
    node {
        echo "Hello world!"
        sh """
        node --version
        java -version
        mvn --version
        npm --version
        """
    }
}

