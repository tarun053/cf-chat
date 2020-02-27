@Library('piper-lib-os') _

node
{
    stage('deploy') {
    cloudFoundryDeploy(
    script: script,
    deployType: 'standard',
        cloudFoundry: [ apiEndpoint: 'https://api.cf.eu10.hana.ondemand.com', appName:'chat_app2', credentialsId: 'CF_CREDENTIALSID', org: 'P1940751883trial_trial', space: 'dev' ]
    deployTool: 'cf_native'
)
}
