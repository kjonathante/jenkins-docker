node {
  stage('First') {
    def ubuntu = docker.image('ubuntu:latest')
    ubuntu.inside {
      checkout scm
      sh 'touch index.html'
      sh 'ls -la > results.txt'
    }
  }
}
