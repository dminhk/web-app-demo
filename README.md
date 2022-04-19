# Simple web app demo

* Ubuntu 20.04
```
  user_data = <<-EOF
    #!/bin/bash
    sudo apt update
    sudo apt update
    git clone https://github.com/dminhk/web-app-demo.git
    sudo apt install apache2 -y
    sudo cp /home/ubuntu/web-app-demo /var/www/html/
    EOF
```
