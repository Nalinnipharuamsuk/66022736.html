pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Nalinipharuamsuk/66022736.html.git'
            }
        }
        stage('Build') {
            steps {
                sh 'cp -r oxer-html/* /var/www/html/'  // คัดลอกไฟล์ไปยังเซิร์ฟเวอร์
            }
        }
        stage('Deploy') {
            steps {
                sh 'systemctl restart apache2'  // รีสตาร์ทเว็บเซิร์ฟเวอร์
            }
        }
    }
}
