pipeline {

agent any

stages {

stage('Checkout') {

steps {

git https://github.com/nikita-px/myrepo2.git

}

}

stage('Publish') {

steps {

publishHTML([

target: [

allowMissing: true,

alwaysLinkToLastBuild: false,

keepAll: false,

reportDir: '.',

reportFiles: 'htmldemo.html',

reportName: 'My html report'

]

])

}

}

}

}
