@Library('piper-lib-os') _

node
{
    stage('deploy') {
    cloudFoundryDeploy(
    script: this
        deployTool: 'cf_native'
        deployType: 'standard'
        cloudFoundry:
            apiEndpoint: 'https://api.cf.eu10.hana.ondemand.com'
            appName:'chat_app2'
            credentialsId: 'CF_CREDENTIALSID'
            org: 'P1940751883trial_trial'
            space: 'dev'
    )
}
}
