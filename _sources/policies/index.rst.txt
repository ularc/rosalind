Policies
########

.. _rosalind_system_use_policies:

Rosalind's System Use Policies
==============================

User Account
-------------

#. Account sharing is prohibited. An account shared amongst multiple users can be a security risk and any such sharing can lead to the suspension of the account.
#. Shared systems like LARCC, BigData, Rosalind, and Zurada should be used mindfully. Negative actions of one user (e.g., excessive number of file transfers leading to network saturation) can negatively impact the other users on the systems.
#. Commercial activities that personally benefit a user and cryptocurrency related work (bitcoin mining) are prohibited on the systems maintained by the Research Computing group. Any activity of this nature when detected will lead to the suspension of the account.
#. Accounts that have not been used for accessing the systems for more than 6-months will be deactivated for security reasons.
#. Users should not create, transmit, or store illegal or inappropriate data on the systems maintained by the Research Computing group.

Storage Use
-----------

#. By default, users will receive a private directory with a quota of ``500GB``.
#. Upon receiving access to Rosalind, users can transfer data via ``SFTP`` (over Port 22) from the University of Louisville Campus network or over the UofL Global Protect VPN. Users that have access to Zurada can also view their files on Rosalind through a mounted directory on login nodes. Before computing with the data stored on Rosalind, the users will need to explicitly transfer the data from Rosalind to the Zurada filesystem (/work directory).
#. Shared directories for projects can be requested on Rosalind. Users can open a :ref:`ticket <user_support_tickets>` with Research Computing to get that set up with discussion on the Quota needed for the group.
 
#. The user ``/home/${USER}`` directory on the Rosalind Server should only be used for bash or SSH configurations and **should not** be used as a primary storage location. Use of the directory is not supported and any files saved there may not be safe from purging.