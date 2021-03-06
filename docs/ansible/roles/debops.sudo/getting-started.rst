Getting started
===============

.. contents::
   :local:


Example inventory
-----------------

The ``debops.sudo`` role is included by default in the ``common.yml`` DebOps
playbook; you don't need to add hosts to any Ansible groups to enable it.


Example playbook
----------------

If you are using this role without DebOps, here's an example Ansible playbook
that uses the ``debops.sudo`` role:

.. literalinclude:: ../../../../ansible/playbooks/service/sudo.yml
   :language: yaml


Ansible tags
------------

You can use Ansible ``--tags`` or ``--skip-tags`` parameters to limit what
tasks are performed during Ansible run. This can be used after a host was first
configured to speed up playbook execution, when you are sure that most of the
configuration is already in the desired state.

Available role tags:

``role::sudo``
  Main role tag, should be used in the playbook to execute all of the role
  tasks as well as role dependencies.


Other resources
---------------

List of other useful resources related to the ``debops.sudo`` Ansible role:

- Manual pages: :man:`sudo(8)`, :man:`sudoers(5)`
