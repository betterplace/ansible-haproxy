# Haproxy for ansible

This role creates a basic haproxy setup.

## Usage

After running this role, create another role that puts a specific configuration
file into `/etc/haproxy/config.pats` and `notify configure haproxy`

Haproxy will assemble all the parts of the config, and restart.

## Caveat

Remember that if you use a wildcard ip for your frontend, surprising things
may happen if someone adds a second frontend
