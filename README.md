# minuto-ansible-playbook

This playbook configures a machine from (almost) scratch to test a media_choice_users repository.

## Installation

+ Host:
	+ You must have a clean Ubuntu installation running on host.
	There should be a ssh server and you must have your key authorized for login.
+ Client:
	+ You must have ansible installed.

## Running

+ At the client, you must configure:
	+ Download the rvm1-ansible submodule: ```git submodule update --init --recursive```
	+ Setup the host ip in the ```hosts``` file
	+ Copy a private/public key pair with access to the github repository to ```keys/```
	+ Run ```ansible-playbook -i hosts site.yml -u root```