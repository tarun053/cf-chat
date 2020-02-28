@Library('piper-lib-local') _

node('master')
{   
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    
stage('build') {
    mtaBuild script: this
}
    stage('deploy') {
    cloudFoundryDeploy script: this
    }
}
