@Library('piper-lib-os') _
node('master')
{
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    
stage('build') {
    mtaBuild(
        script: this,
        verbose: 'true' )
}
    stage('deploy') {
    cloudFoundryDeploy( 
        script: this,
        verbose: 'true' )
    }
}
