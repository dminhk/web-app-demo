# Simple web app demo

* Amazon Linux 2 AMI 
```
  user_data = <<-EOF
    #!/bin/bash
    sudo yum install httpd -y
    sudo yum install git -y
    sudo rm -rf /var/www/html/*
    sudo git clone https://github.com/dminhk/web-app-demo.git /var/www/html/
    sudo systemctl start httpd
    sudo systemctl enable httpd
    EOF
```
