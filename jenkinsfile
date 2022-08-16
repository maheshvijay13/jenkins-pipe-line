pipeline {
    agent any
    environment{
        name='Mahesh'
    }
    parameters{
        string(name : 'person', defaultValue: 'Mahesh', description: 'test')
    }

    stages {
        stage('Test') {
            steps {
                echo 'Test-Hello World';
            }
        }
         stage('Build') {
            steps {
                echo 'Build -Hello World';
                echo "%person%";
            }
        }
         stage('Deploy') {
            steps {
                echo 'Deploy-Hello World'
            }
        }
    }
    post{
        always{
            echo 'Always'
        }
        failure{
            echo 'Failure'
        }
        success{
             echo 'Success'
        }
    }
}
