.. image:: https://travis-ci.org/ajite/docker-postgres-client.svg?branch=master
    :target: https://travis-ci.org/ajite/docker-postgres-client
.. image:: https://coveralls.io/repos/ajite/docker-postgres-client/badge.svg?branch=master&service=github :target: https://coveralls.io/github/ajite/docker-postgres-client?branch=master
.. image:: https://codeclimate.com/github/ajite/docker-postgres-client/badges/gpa.svg
   :target: https://codeclimate.com/github/ajite/docker-postgres-client
   :alt: Code Climate

docker-postgres-client
======================
I created this library to work with different version of Docker Postgres without having the need to change my Postgres client.

To install and use it type the command below:

.. code-block:: bash

    pip install docker-postgres-client

You will then have four new commands available in your shell: dpsql, dcreatedb, ddropdb, and dpg_dump. They allow you to connect, create, drop, dump, and import a database. If you want to add additional features feel free to fork this repository and make a merge request.

All the bash command have -c (container) option  that you can use like below:

.. code-block:: bash

    dpsql -c CONTAINER_NAME -U user_name

Last but not least all the scripts contain a useful help message to know how to use them.

.. code-block:: bash

    dpsql --help
