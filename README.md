example conf:

    input {
      	tcp{
    		jdbc_driver_library => "/root/mysql-connector.jar"
   		jdbc_driver_class => "com.mysql.jdbc.Driver"
    		jdbc_connection_string => "jdbc:mysql://192.168.65.128:3306/hoolis"
    		jdbc_user => "root"
    		jdbc_password => "root"
    		port => "2181"
    		user_limit => "1M"
      	}
    }
    output{
    	stdout{
    		codec => rubydebug``
    	}
    }
    
