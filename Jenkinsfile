pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        sh 'echo "Hello World"'
        junit(testResults: 'out/target/product/avsdm/obj/ROBOLECTRIC/**/coverage-output.xml', healthScaleFactor: 1, keepLongStdio: true)
      }
    }

  }
}