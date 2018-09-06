# beakerx-xeus-cling

Docker files for a docker image which integrate beakerx and xeus-cling to provide almost all the popular language support to jupyter. 

This image is simply an installation of [xeus-cling](https://github.com/QuantStack/xeus-cling) based on [beakerx](https://github.com/twosigma/beakerx).

### How to run it

1. Using docker command to run it
    `docker run -d -p 8888:8888 liudonghua123/beakerx-xeus-cling`
2. Using docker-compose command to run it (prefered)
    write a docker-compose.yml which contains like
    ```
	version: '2'

	services:
	    beakerx-xeus-cling:
	        image: liudonghua123/beakerx-xeus-cling:latest
	        ports:
	            - "8888:8888"
	        restart: always
    ```

### License

MIT
