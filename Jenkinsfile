node{
   stage('SCM Checkout'){
     git 'https://github.com/Marvel-Avenger/my-app/'
   }
   stage('Compile-Package'){
      // Get maven home path
      def mvnHome =  tool name: 'maven-3', type: 'maven'   
      sh "${MAVEN_HOME}/bin/mvn package"
   }
   stage('Email Notification'){
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts
      Thanks
      Hari''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'nandurilaxman9@gmail.com'
   }
}
