@Library('piper-lib-os') _
tools {
nodejs 'NodeJS8.10.0'
}
node
{
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    
stage('build') {
    mtaBuild script: this
}
    stage('deploy') {
    sh '''
    cloudFoundryDeploy script: this
    '''
    }
}
