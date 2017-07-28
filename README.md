# Docker LAMP multi container

This will copy all the Docker files to create the php7 apache2.4 and mysql5.7 container.
    
``git clone git@github.com:germancin/docker-lamp-env.git wfm-dev-env``
    
``cd wfm-dev-env``
       
This will copy all the files for WFM project.
       
``git clone git@github.com:PeopleStrategy/Yellow-TimeandLabor.git``

This will build the containers.
    
``docker-compose up -d``

### Database setup.
Copy ``wfm-db.sql`` file into ``/wfm-dev-env/mysql/database/``

Get ``wfm-db.sql`` from shared folder ``/Open/wfm-assets/``

Open kitematic and get into ``mysql-container`` shell 

Now run command ``ls`` to list all files and you should see ``wfm-db.sql``
 
``mysql -uroot -ppassword``

``mysql> source wfm-db.sql ``

### Git Working Branch.
Open your Docker Quick start terminal and get into the project folder.

``cd /wfm-dev-env/Yellow-TimeandLabor/``

Checkout the the working project branch

``git checkout EHCMS-1424-MASTER``

Branch out from ``EHCMS-1424-MASTER``

``git checkout -b EHCMS-1424-CHILD-task-description EHCMS-1424-MASTER``

Done!! You can start pushing code ;) 

