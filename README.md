# DESCRIPTION

### What is it?

This is a project that automatically provisions a compute engine for high performance computing (HPC) applications. It uses Google's cloud platform.

### Main Components

The main components of this project are:

* A shell script "deploy.sh": this handles the entire process of provisioning the resources and deleting it after a set time.
* A yaml config file that holds the configuration information for the compute engine.
* A machineTypesList.json file generated by making the api explorer call https://compute.googleapis.com/compute/v1/projects/{project}/zones/{zone}/machineTypes to get the list of supported machines. {project} and {zone} should be replaced by the project name and gcp zone respectively.
* A startup.sh file that sets up the vm with the required applications after it has been provisioned.

## License
This work is published under the terms of MIT License. See LICENSE file for the terms of this license.
