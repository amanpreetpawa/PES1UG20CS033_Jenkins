pipeline{
agent any stages{
stage('Building Phase'){ steps{
sh 'make -C /var/jenkins_home/workspace/PES1UG20CS033'
echo 'Deployed Successfully' }
}
stage('Execution Phase'){
steps{
sh './hello_exec'
echo 'Executed Successfully'
} }
stage('Deployment Phase'){ steps{
echo 'Push somewhere' }
} }
post{ failure{
echo 'Pipeline Failed' }
} }
