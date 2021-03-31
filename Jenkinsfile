
node {
  stage('checkout sources') {

        git url: 'https://github.com/ccoats-cscc/specialtopics-ci-lab'
  }
  try {

    stage('Build') {

        withMaven (maven: 'maven3') {
            sh "mvn package"
        }
    }
  } finally {
        junit 'target/**/*.xml'
  }
}
