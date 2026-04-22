Getting Started
###############

.. _usage-agreemet:

Usage Agreement
===============

Please ensure that you have read :ref:`Rosalind's System Use Policies <rosalind_system_use_policies>`
and have agreed to it before requesting an account.

Connecting to Rosalind
======================

There are a couple of ways to connect and utilize the Rosalind system. Please note, that you must be connected to either the University of Louisville campus network or the UofL Global Protect VPN.

SFTP
----

**Client - Preferred**

  #. Open your preferred SFTP client (e.g., CyberDuck and Filezilla)
  
  #. Enter the following information in the client
  
      .. list-table:: SFTP Client Info
          :header-rows: 1

          * - Key
            - Value
          * - Host
            - rosalind.rc.louisville.edu
          * - Username
            - your ULINK ID (i.e., fmlast01)
          * - Password
            - Your University of Louisville Password
          * - Port
            - 22
      
      .. note::
        If your client needs a URL rather than ``host`` + ``port`` then you can try ``sftp://rosalind.rc.louisville.edu`` instead
  
  #. Make sure you check your phone for a DUO push notification

**Command Line**
  
  #. Open a terminal session

  #. Type the command:
  
      .. code-block::
  
          sftp ${USER}@rosalind.rc.louisville.edu
  
  #. Enter your UofL password, and check your phone for a DUO push.

  This will start an SFTP session, and after login you will be in a private directory on Rosalind. You can use the following commands to interact with the session:
  
  .. list-table:: SFTP commands
      :header-rows: 1

      * - Command
        - Meaning
      * - ls
        - List files and directories
      * - cd
        - Change directory
      * - pwd
        - Display current directory
      * - get
        - Download a file from the Data Store
      * - put
        - Upload a file to the Data Store
      * - mkdir
        - Create a directory
      * - rmdir
        - Remove an empty directory
      * - rm
        - Delete a file

  Example

  .. code-block:: bash

    C:\Users\fmlast01> sftp fmlast01@rosalind.rc.louisville.edu
    This system is the property of the University of Louisville.

    Use of the system is for authorized users only. It is the policy of the
    University to protect and safeguard the protected health information,
    created, acquired and maintained in accordance with the Privacy
    Regulations promulgated pursuant to the Health Insurance Portability
    and Accountability Act of 1996 and all applicable state laws.

    Use of your account constitutes your approval and acceptance of this
    agreement. Acceptance of this agreement is a condition of use.

    IMPORTANT!

    USER DOCUMENTATION: https://ularc.github.io/rosalind/

    Please type your University of Louisville password.
    REMARK: Even if you don't see any characters in the
    prompt, your input is recorded.

    AFTER TYPING YOUR PASSWORD, check your phone for a
    DUO prompt.

    fmlast01@rosalind.rc.louisville.edu's password:
    Autopushing login request to phone...
    Success. Logging you in...
    Connected to rosalind.rc.louisville.edu.
    sftp> 
    sftp> pwd
    Remote working directory: /mnt/rosalind/private/fmlast01
    sftp> 
    sftp> ls
    sftp> 
    sftp> put C:\Users\fmlast01\Downloads\Image.jpg .
    Uploading C:/Users/fmlast01/Downloads/Image.jpg to /mnt/rosalind/private/fmlast01/./Image.jpg
    Image.jpg                                                                                                                        100% 7912KB   1.5MB/s   00:05
    sftp> 
    sftp> get /mnt/Rosalind/private/fmlast01/./Image.jpg .\mytestimage.jpg
    Fetching /mnt/rosalind/private/fmlast01/./Image.jpg to ./mytestimage.jpg
    Image.jpg                                                                                                                        100% 7912KB 517.7KB/s   00:15
    sftp> 
    sftp> ls
    Image.jpg
    sftp> 
    sftp> pwd
    Remote working directory: /mnt/rosalind/private/fmlast01
    sftp> 
    sftp> exit

SSH
---
  #. Open your SSH client of choice (or a terminal session)
  
  #. Use the following information to connect
      .. list-table:: SSH Information
          :header-rows: 1
          
          * - Key
            - Value
          * - Host
            - rosalind.rc.louisville.edu
          * - Username
            - your ULINK ID (i.e. fmlast01)
          * - Password
            - Your University of Louisville Password
          * - Port
            - 22
  
  #. Make sure you check your phone for a DUO push notification
  
.. note::
    
  Upon connecting to Rosalind, by default, you will be in your private directory.