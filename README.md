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