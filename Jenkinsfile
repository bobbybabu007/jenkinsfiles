node {
    def mvnHome = tool 'M3'

    stage('Checkout') {
 #       checkout scm
        sh "git clone https://github.com/bobbybabu007/jenkinsfiles.git code && cd code && git checkout 1-scripted"
    }

    stage('Build') {
        sh "${mvnHome}/bin/mvn -B package"
    }
}
