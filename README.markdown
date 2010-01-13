This is made to work alongside of a Rails application

 - git clone git://github.com/grosser/mysql_proxy_logging.git
 - cd mysql_proxy_logging
 - sudo apt-get install mysql-proxy
 - database.yml: change port to 4040, host to 127.0.0.1
 - ./record
 - database.yml: change back port/host
 - ./replay logfile path_to_rails_root times sleep_between_runs (e.g. replay mysql.log /srv/my_app/current 20 0.1)
