
node {
  stage('checkout sources') {

        git url: 'https://github.com/ccoats-cscc/specialtopics-ci-lab'
  }

  stage('Build') {

    withMaven (maven: 'maven3') {
        sh "mvn package"
    }

    echo "hello"
  }
  // you should add a test report here
}
