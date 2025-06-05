# rhis-builder-provisioner

Fork it. Clone it. Configure it. Test it. Change it. Commit it. Create a PR.

***

#### Helping out
I know that most of you have experience with these things, but we also work with people with less experience. So, please bear with us if a lot of items that you know are spelled out. If you have any comments, tips, tricks or suggestions to add to the documentation or README.md file, PRs are greatly appreciated. Let's share the wealth!

If you haven't been there yet, please visit the [rhis-builder-provisioner wiki](https://github.com/parmstro/rhis-builder-provisioner/wiki) first

See rhis-builder-vault-SAMPLE repo for secrets definitions.
***
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
