pipeline {
    agent any
    stages {
        stage('Upload to AWS S3') {
            withAWS(region: 'us-west-2') {
                s3Upload(file: 'index.html', bucker: 's3bucketforjenkinsaravind', path: 'static/index.html')
            }
        }
    }
}