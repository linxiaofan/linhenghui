pipeline {
  agent any
  stages {
    stage('parent') {
      parallel {
        stage('parent') {
          steps {
            echo 'parent'
            echo 'child1'
          }
        }
        stage('child') {
          steps {
            echo 'child1'
          }
        }
        stage('child2') {
          steps {
            echo 'child2'
          }
        }
      }
    }
  }
}