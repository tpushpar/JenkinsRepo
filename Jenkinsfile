pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
          stage('One') {
            steps {
                echo 'Stage One - Devlopment'
            }
          stage('Two') {
            steps {
                echo 'Stage Two - Build'
            }
        }
         stage('Three') {
           parallel{
             stage('Unit Testing'){
               steps {
                echo 'Parallel Stage - Unit Testing'
                }
             }
             stage('Integration Testing'){
               steps {
                echo 'Parallel Stage - Integration Testing'
               }
            }
         }
    }
}
