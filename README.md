# rhis-builder-provisioner


Use the container!

In an effort to streamline building and using an RHIS environment, we have moved provisioner into a container. This has resulted in consumers getting to a working environment **way** faster. The rhis-provisioner-9 container build is based on RHEL UBI 9 and has all of the code dependencies and all of the ansible code for all of the rhis-builder projects baked in, plus has the example.ca sample configuration for the whole environment. We are working to make "Life is Better with RHIS" a reality. 

You will soon be able to pull the rhis-provisioner-9 container from an official Red Hat repository. In the meantime please access to the [rhis-provisioner-container](https://github.com/parmstro/rhis-provisioner-container) repository to build a container from source.

There is still a small bit of work to get the provisioner ready to deploy the rhis environment.
This project is still valuable to set up the inventory project, git variables and local hosts entries to make it easier to run the container mode.

***

#### Helping out
I know that most of you have experience with these things, but we also work with people with less experience. So, please bear with us if a lot of activities that you know well are spelled out. If you have any comments, tips, tricks or suggestions to add to the documentation or README.md file, PRs are greatly appreciated. Let's share the wealth!

If you haven't been there yet, please visit the [rhis-builder-provisioner wiki](https://github.com/parmstro/rhis-builder-provisioner/wiki) first

See [rhis-builder-inventory](https://github.com/parmstro/rhis-builder-inventory) repo for all sample configurations and secrets definitions.

## What you will need at a minimum:
- a plan! What sort of environment do you want to build? For a sample - example.ca - see the wiki
VMs, Baremetal or cloud instances for:
- a node to run the rhis-provisioner-9 container
- a node for identity management
- a node for satellite

That gets you off the ground, to get flying you will need:
- more baremetal nodes, or 
- a supported hypervisor environment, or 
- a supported cloud environment, or 
- all of the above

to build out the rest of your architecture

## See the [Wiki for Instructions on getting started](https://github.com/parmstro/rhis-builder-provisioner/wiki)
