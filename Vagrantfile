Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.network "public_network", bridge: "en1: Wi-Fi (AirPort)"
  config.vm.hostname = "fdm-box"

  #Provisioning Script
  config.vm.provision "shell", path: "provision.sh"

  #Synced Folders for Windows Host
  #config.vm.synced_folder "C:\\Users\\trainee1.TRNNYC30534\\Documents\\workspace", "/opt/tomcat/workspace"     #Eclipse Workspace Location will be synced with /opt/tomcat/workspace
  #config.vm.synced_folder "C:\\Users\\trainee1.TRNNYC30534\\Documents\\workspace\\IssueTrackingSystem\\assets", "/opt/tomcat/webapps/IssueTrackingSystem/assets"     #Tomcat Assets location of Eclipse Web App
  #config.vm.synced_folder "C:\\Users\\trainee1.TRNNYC30534\\Documents\\workspace\\IssueTrackingSystem\\web", "/opt/tomcat/webapps/IssueTrackingSystem/web"     #Tomcat Web location of Eclipse Web App

  #Port Forwarding for Vagrant Share
  #config.vm.network "forwarded_port", guest: 8080, host: 8080, id: "tomcat"

end
