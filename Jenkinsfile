@Library('piper-lib-local') _
node('master')
{
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    
stage('build') {
    mtaBuild(
        script: this,
        mtaBuildTool: 'Classic',
        verbose: 'true' )
}
    stage('deploy') {
    cloudFoundryDeploy( 
        script: this,
        verbose: 'true' )
    }
}
