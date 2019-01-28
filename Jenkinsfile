#!/usr/bin/env groovy

@Library('piper-library-os-experimental') _

stage ('node') {
    node {
	deleteDir()
	checkout scm
        setupCommonPipelineEnvironment script: this
	nodeBuild script: this
    }
}
