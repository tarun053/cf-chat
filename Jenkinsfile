@Library('piper-lib-os') _

node('jenkins233slave'){
  stage('Deploy')   {
      cloudFoundryDeploy(
      script:this, 
      verbose:true)
  }
}
