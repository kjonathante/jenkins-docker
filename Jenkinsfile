node {
  stage('First') {
    checkout scm
    def browsers = docker.build('browsers:latest','-f docker/browsers/Dockerfile .')
    browsers.inside {
      sh 'touch index.html'
      sh 'ls -la > results.txt'
    }
  }
}
