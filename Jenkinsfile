pipeline{
agent any
stages{
stage('Clone Repository'){
steps{
git branch:'main', url : 'https://github.com/AmeyM02/PES2UG20CS037_Jenkins.git' }
}
stage('Build'){
steps{
sh 'make -C main' }
}
stage('Test'){
steps{
sh 'main/hello_exec' }
}
stage('Deploy'){
steps{
sh 'echo "Running file" && main/hello_ex' }
}
}
post{
failure{
sh 'echo "Pipeline Failed"' }
}
}
