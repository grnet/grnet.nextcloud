grnet.nextcloud Ansible collection
==================================

A collection of modules to setup nextcloud on Debian.

Installation
------------

::

  ansible-galaxy collection install \
      git+https://github.com/grnet/grnet.nextcloud.git

How to use
----------

The repository has an :file:`examples` directory. Use it like this:

1. Ensure you have a valid domain name on which to install Nextcloud
   (it's hard to use an invalid domain name because certbot will not
   work properly).
2. Ensure the collection is installed as explained in the "Installation"
   section above.
3. Copy :file:`examples/nextcloud-deploy` elsewhere and go there to make
   changes.
4. Find all instances of ``example.com`` and modify them as needed.
5. Run the playbook: ``ansible-playbook site.yml``.

Reference
---------

.. toctree::
   nextcloud
   collabora
   :maxdepth: 1
   :caption: Roles:

.. toctree::
   copyright
   :maxdepth: 1
   :caption: Meta:
