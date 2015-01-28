opsworks stack custom json:


{  
    "rabbitmq": {  
	 "cluster": true,  
    	 "erlang_cookie": "<any random alphanumeric string will do>"  
    },    
    "rabbitmq_cluster": {  
    	"user": "<rabbitmq username here>",  
    	"password": "<rabbitmq password here>"  
    }    
}  


For SSL:   
{    
   "rabbitmq": {
     "web_console_ssl": true,
     "web_console_ssl_port": "15671"
   }  
}  
     

CmdLine Notes:       
     
rabbitmqctl change_password username password       
rabbitmqctl set_user_tags username "tags"    
rabbitmqctl set_permissions -p / username "*" ".*" ".*"         
     
