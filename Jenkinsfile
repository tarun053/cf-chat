@Library('piper-lib-os') _

node('jenkins233slave'){
  stage('Deploy')   {
      cloudFoundryDeploy(
      script:this, 
      cloudFoundry: [apiEndpoint: 'https://api.cf.eu10.hana.ondemand.com', appName:'chatapp2', credentialsId: 'CF-devsecops20', org: '47dac577trial', space: 'dev'],
      deployTool: 'cf_native',
      verbose:true)
  }
}
