@Library('piper-lib-local') _

node('master'){
  stage('Prepare')   {
      deleteDir()
      checkout scm
      setupCommonPipelineEnvironment script:this
  }
}
