
#About this repository
It contains the source code for the cc-revisionlog solution and other two dependencies:
	* efk - which stands for elasticsearch, fluentd and kibana. Actually we replaced the logstash app with fluentd and kept the rest of the architecture as we found it in (this repo)[https://github.com/deviantony/docker-elk]
	* demo-app is a small web application where requests comming from our reverse proxy will be forwarded. More details can be found [here](https://github.com/docker/example-voting-app)
	


#### For being able to run these docker images locally you might need to follow this tutorial: [DED0033 - CC Development Environment Installation Manual](https://bitbucket/projects/ENET/repos/environment/browse/docs/DED0033-Development-environment-installation-manual.md)

The demo-app will be running at [http://localhost:5000](http://localhost:5000), and the results of the demo-app will be at [http://localhost:5001](http://DOCKER_MACHINE_IP_ADDRESS:5001).
The nginx reverse proxy will be running at [http://{DOCKER_MACHINE_IP_ADDRESS}:8080](http://localhost:8080) and it will forward your requests on port 5050 (to the demo-app).

##Architecure: