pipeline{
    agent any
    stages{
       stage('Clone') {
    steps {
        git branch: 'main', url: 'https://github.com/Navajeevan-99/Static-Article.git'
    }
}
stage('Deploy') {
    steps {
        sh '''
        mkdir -p /var/www/html/build-$BUILD_NUMBER
        cp -r * /var/www/html/build-$BUILD_NUMBER/
        '''
    }
}

    }
}