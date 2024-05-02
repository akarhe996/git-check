pipeline {
  agent any
  stages{
    stage('Build') {
      steps {
        git branch: 'main', url: 'https://github.com/akarhe996/python_test.git'
        sh '/usr/bin/python app.py'
      }
    }
    stage('mail') {
      steps {
        mail bcc: '', body: 'pipeline executed successfully', cc: '', from: '', replyTo: '', subject: 'build success', to: 'akash.karhe1992@gmail.com'
      }
    }
  }
}
