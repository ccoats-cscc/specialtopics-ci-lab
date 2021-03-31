
node {
  stage('checkout sources') {
        // You should change this to be the appropriate thing
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
