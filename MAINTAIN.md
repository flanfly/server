Maintenance
===========

Roles
-----

server: Basic configuration for new servers, mostly installs admin accounts and docker.

public: Public facing services like email, jabber, websites.

Update
------

The docker containers are updated each time this runs:

ansible$ ansible-playbook plays/public.yml

The container should update if its configuration changes or the base
image is updated.

Note that site.yml includes this.
