pipeline {
    agent any
    stages { 
        stage('Outer Stage 1') {
            when {
                branch 'develop'
            }
            stages {
                stage('Inner Stage 1-1') {
                    steps {
                        echo 'Executing Inner Stage 1-1'
                    }
                }
                stage('Inner Stage 1-2') {
                    steps {
                        echo 'Executing Inner Stage 1-2'
                    }
                }
            }
        }
        stage('Outer Stage 2') {
            when {
                branch 'test'
            }
            stages {
                stage('Inner Stage 2-1') {
                    steps {
                        echo 'Executing Inner Stage 2-1'
                    }
                }
                stage('Inner Stage 2-2') {
                    steps {
                        echo 'Executing Inner Stage 2-2'
                    }
                }
            }
        }
      stage('Outer Stage 3') {
            when {
                branch 'main'
            }
            stages {
                stage('Inner Stage 3-1') {
                    steps {
                        echo 'Executing Inner Stage 3-1'
                    }
                }
                stage('Inner Stage 3-2') {
                    steps {
                        echo 'Executing Inner Stage 3-2'
                    }
                }
            }
        }
    }
}
