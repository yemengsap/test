#!/usr/bin/env groovy

@Library('piper-library-os-experimental') _

stage ('node') {
    node {
	deleteDir()
	checkout scm
        setupCommonPipelineEnvironment script: this
	npmExecute(script: this)
	npmExecute(script: this, npmCommand: 'run build') { sh "node --version && npm --version"}
    }
}
