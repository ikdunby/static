pipeline {
    agent any
    stages {
       stage('Upload to AWS') {
             steps {
                 
                 s3Upload(file:'index.html', bucket:'udacity.jenkins', path:'index.html')
                 sh 'echo "Uploaded the file"'
                 sh '''
                     echo "Multiline shell blablabla"
                     ls -lah
                     '''
             }
        }
    }
}