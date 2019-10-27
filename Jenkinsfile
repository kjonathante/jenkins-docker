node {
  stage('First') {
    def browsers = docker.build('browsers:latest','-f docker/browsers/Dockerfile')
    browsers.inside {
      checkout scm
      sh 'touch index.html'
      sh 'ls -la > results.txt'
    }
  }
}
