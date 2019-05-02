#!groovy
pipeline{
    agent any
    stages {
        stage ("Build"){
            steps{
                echo 'Building'
                git 'https://github.com/GuilhermeBuenoMartins/indra20190417.git'
            }
        }
        stage ("Test"){
            steps{
                sh '''
                pip install python-jenkins
                python -m pip install --upgrade pip
                pip install virtualenv
                virtualenv env
                env//s//activate
                
                '''

            }
        }
    }
}
