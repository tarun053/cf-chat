@Library('piper-lib-os') _

node('jenkins233slave'){
  stage('Prepare')   {
      checkout scm
      setupCommonPipelineEnvironment script:this
  }
  stage('build') {
    mtaBuild(
        script: this )
  }
    stage('deploy') {
    cloudFoundryDeploy( 
        script: this,
        verbose: 'true' )
    }  
}
