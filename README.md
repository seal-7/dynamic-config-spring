#Reference
https://spring.io/guides/gs/centralized-configuration/
#How to change config
Config server updates config based on git commit in folder config-store
For updating the config in client you will have to invoke api actuator/refresh after doing commit in config-store.

	$ curl localhost:8080/actuator/refresh -d {} -H "Content-Type: application/json"
