node ("docker-agent-jnlp") {
  stage('Hello')
  {
    echo 'Hello World'
  }

  stage('Prepare') {

    // Get repository
    checkout scm
  }
  stage('Build') {
    built_image = docker.build("${JOB_NAME}:${BUILD_NUMBER}")
  }
  stage('Sleep') {

    // Get repository
    sleep(60)
  }
}
