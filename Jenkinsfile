@Library('piper-lib-os') _
node('master')
{
 stage('prepare') {
            deleteDir()
            checkout scm
            setupCommonPipelineEnvironment script:this
        }
}
