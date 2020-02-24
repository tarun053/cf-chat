@Library('piper-lib-os') _
node
{
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    
stage('build') {
    buildExecute script:this, buildTool: 'mta'
    mtaBuild script: this
}
    stage('deploy') {
    sh '''
    cloudFoundryDeploy script: this
    '''
    }
}
