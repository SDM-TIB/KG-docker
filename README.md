# KG-docker

Run this command to start the docker container

`docker run -d --name iASIS-KG -v '/data/asakor/iASIS_KG/all_21_3_19/data:/app/data/' -p 11686:8890 -p 1616:1111 asakor/iasiskgnt:latest`

change this path to the path in your machine where you clonned the repository:
`/data/asakor/iASIS_KG/all_21_3_19/data`


Fell free to change the ports (11686, 1616), and the container name (iASIS-KG)

To check the status of loading the data into the endpoint, run:

`docker logs -f iASIS-KG`

When the data is done loading you will see the message:
`temp data deleted`

