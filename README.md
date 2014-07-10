# Replicating MySQL Cluster Demo

This demo is a lightweight bash script to bring together two Docker Containers to create a replicating MySQL cluster for testing / development purposes.

It is as simple as running ./start_cluster, passing in the number of slaves you want in your cluster like so:

```
./start_cluster -n 2
```

The script will pull a master image and a slave image from the docker hub and will start one master and as many slaves as you specify, with replication set up and working out of the box.

Ideal for testing read-write splitting in your web application.

# Requirements

* Docker
* Internet

# License

MIT License
