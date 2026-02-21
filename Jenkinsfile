pipeline {
agent any
stages {
stage('clone') {
steps {
git branch:'main', url: 'https://github.com/Shivashankar-2004/Calculator.git';
}
}
stage('compile') {
steps {
sh 'javac Calculator.java'
}
}
stage('build') {
steps {
sh 'java Calculator 25 5'
}
}
stage('test'){
steps{
sh 'java calculator 30 -5'
}
}
stage('Deploy') {
steps {
echo 'Deploy completed'
}
}
}
}
