# Ansible-unitspec

Ansible toolbelt for role and playbook unit testing

## What we want

We want to be able to:

## Run unit tests

We want to be able to run unit tests on 
- Ansible roles
- Ansible playbooks

It should be simple to bootstrap, and the tool interface should be
identical whatever we are testing.

## Run on different OSes

We want to run on deb and rpm based systems.

## Check idempotency

We want to be able to check role or playbook idempotency.

## Ansible version

We want to be able to run our tests against a specific (or multiples)
Ansible versions.

Ansible used for the test could be installed with the OS package
manager, or from checkout.

## Access to ansible CLI

We want access to the ansible CLI so we can inject extra vars, or
restrict test to a specific tag.

## Branch handling

The testing tool shoul dbe able to handle branches, e.g. test a playbook
against a specific role branch, or vice-versa.

Ultimately, we want to be able to test a role on it's devel (or feature)
branch, before rebasing/merging on master.

## Dependencies

We want the tool to retrieve dependencies automatically from
`meta/main.yml` when available.

We want to be able to wipe those dependencies and pull them again if
needed.

Those deps could live anywhere (hypervisor, host, docker volume
container, source repos, ...).

## Platforms

We wahnt to be able to test in Vagrant, Docker, both (docker-machine),
Travis, whatever-CI.


