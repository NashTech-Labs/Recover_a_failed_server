# Recover_a_failed_server
In this playbook, we first define some variables, including the location and name of the latest backup, the hostname and IP address of the new server to be provisioned, and the username and password for the new server.

The playbook then downloads the latest backup, extracts it to /tmp, provisions a new openstack server, waits for the server to be available, copies the backup to the new server, and restores the backup on the new server.