# nginx Tutorial on Unbuntu

## Installation

  1. setup
    * install lynx: `sudo apt-get install lynx`
    * install ssh if not installed: `sudo apt-get install ssh`

  2. install
    * `sudo vi /etc/apt/sources.list`
    * add ngix repos to the end of the file, and save
      ```
      deb http://nginx.org/packages/ubuntu/ trusty nginx

      deb-src http://nginx.org/packages/ubuntu/ trusty nginx
      ```
    * `sudo apt-get update` to get the packages from list. but you will get error on signature.
    * add signature key
      ```
      wget http://nginx.org/keys/nginx_signing.key

      sudo apt-key add nginx_signing.key
      ```
    * update `sudo apt-get update`
    * `sudo apt-get install nginx`
    * verify by `nginx -v`
