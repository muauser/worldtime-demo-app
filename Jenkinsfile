pipeline
{
agent any
stages{
stage('Build Application'){
steps{
bat 'mvn clean install'
}}

stage('Test MUnit Application'){
steps{
bat 'mvn test'
}}

stage('Deploy Application to Mulesoft CloudHUb'){
steps{
bat 'mvn package deploy -DmuleDeploy'
}}

stage('Perform Regression Testing'){
steps{
bat 'C:\\Users\\aadhya\\AppData\\Roaming\\npm\\newman run C:\\Newman\\WorldTime-Demo.postman_collection.json --disable-unicode'
}}

}

}