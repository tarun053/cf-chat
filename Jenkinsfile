@Library('piper-lib-os') _

node('master'){
  stage('Prepare')   {
      checkout scm
      setupCommonPipelineEnvironment script:this
  }
  stage('build') {
    mtaBuild(
        script: this )
  }
}
