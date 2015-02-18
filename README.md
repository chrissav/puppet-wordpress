This is a clone of jonhadfield/puppet-wordpress

Changes to wordpress directories and files for custom install.
Remove DB class and implement new parameter wordpress_db_hostname to connect to AWS DB.

Implementation:

    class {
      wordpress:
      wordpress_db_name =>      "<name of database>",
      wordpress_db_user =>      "<database user>",
      wordpress_db_password =>  "<database password>"
      wordpress_db_hostname =>  "<database hostname>"
    }
