pipeline {
  agent any
  enviroment {
    APP_NAME = "demo"
  }
  stages {
    stage("Build") {
      enviroment {
        BUILD_MODE = 'production'
      }
      steps {
        sh 'echo $APP_NAME $BULD_MODE'
      }
    }
  }
}
  
