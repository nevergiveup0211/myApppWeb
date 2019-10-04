node{
  stage('SCM Checkout'){
    git 'https://github.com/nevergiveup0211/myApppWeb.git'
  }
  stage('Compile - Package'){
  bat label: '', script: 'mvn clean package deploy'
  }
  stage('Email Notification'){
    
    mail bcc: '', body: 'Maven Jenkins file', cc: '', from: '', replyTo: '', subject: 'Jenkins file', to: 'nevergiveup0211@gmail.com'
  }
