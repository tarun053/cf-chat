@Library(https://github.com/SAP/jenkins-library) _

node
{
    stage('deploy') {
    cloudFoundryDeploy(
    script: this,
    verbose: 'true',
    deployType: 'standard',
    cloudFoundry: [apiEndpoint: 'https://api.cf.eu10.hana.ondemand.com', appName:'chat_app2', credentialsId: 'CF_CREDENTIALSID', manifest: 'manifest', org: 'P1940751883trial_trial', space: 'dev'],
    deployTool: 'mtaDeployPlugin'
)
}
}
