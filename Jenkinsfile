pipeline
{
agent any
stages{
stage('Build Application'){
steps{
bat 'mvn clean install'
}}

stage('Deploy Application to Mulesoft CloudHUb'){
steps{
bat 'mvn package deploy -DmuleDeploy'
}}

stage('Perform Regression Testing'){
steps{
bat 'C:\\Users\\aadhya\\AppData\\Roaming\\npm run C:\\Newman\\WorldTime-Demo.postman_collection.json --disable-unicode'
}}

}

}