@Library('piper-lib-os') _
node('jenkins233slave')
{
    stage('deploy') {
    cloudFoundryDeploy( 
        script: script,
        verbose: 'true' )
    }
}
