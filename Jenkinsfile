@Library('piper-lib-os') _

node('master'){
  stage('Prepare')   {
      deleteDir()
      checkout scm
      setupCommonPipelineEnvironment script:this
  }
}
