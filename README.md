# rhis-builder-provisioner

This repository contains the code that configures the host that will provision an rhis infrastructure. 
There are really two ways to approach provisioning the rhis environment. 
1) Create a workstation, or other node, that has ansible core and the related collections necessary to run our projects. (Like deploying Openshift)
2) Create an aap all-in-one server that we can synchronize all the projects to and create the necessary workflows to build the rhis. This AAP server will (Like creating an under-cloud a la Openstack)

We will initially pursue method 1 as this is the simplest. At a future date we will investigate 2 as we need to control the integrated deployment using workflows.

### Limitations
- today this supports and is tested on an enterprise linux host (happy to accept pull requests supporting MacOS or other systems as the provisioner)
- Deployment is on RHEL9

## What you will need at a minimum:
- a plan! What sort of environment do you want to build? For a sample - example.ca - see the wiki
- a node to serve as the provisioner (virtual or baremetal)
- a node for identity management
- a node for satellite
  and
- more baremetal nodes, or a supported hypervisor environment, or a supported cloud environment to build out the rest of your architecture

## See the [Wiki for Instructions on getting started](https://github.com/parmstro/rhis-builder-provisioner/wiki)
