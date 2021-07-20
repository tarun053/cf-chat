@Library('piper-lib-local') _
node('master')
{
 stage('prepare') {
            deleteDir()
            checkout scm
            setupCommonPipelineEnvironment script:this
        }
}
