# Magento2_project
Setting up a Debian 12 server with specific components and configurations for hosting Magento 2

The assignment involves setting up a Debian 12 server with specific components and configurations for hosting Magento 2. Here's a summary of the tasks:


1. Install Components:
   - PHP 8.1: This is the programming language that Magento 2 is built on.
   - MySQL 8: The database management system for storing Magento data.
   - NGINX: A web server software to serve Magento's web pages.
   - Elasticsearch: Used for advanced search functionality in Magento.

2. Install Magento 2:
   - Install the latest Magento 2 version using Composer. Include Sample Data for testing purposes.
   - Configure Magento to work with Elasticsearch.
   - Use the domain "test.mgt.com" and ensure that localhost resolves to "127.0.0.1 test.mgt.com."

3. Redis Configuration:
   - Install Redis-Server.
   - Configure Magento to use Redis for caching and session storage instead of the file system.

4. User and Group Setup:
   - Create a user named "test-ssh."
   - Create a group named "clp."
   - Change ownership of all files to the user "test-ssh" and group "clp."

5. NGINX Configuration:
   - Configure NGINX to run as the user "test-ssh."

6. PHP-FPM Pool:
   - Create a PHP-FPM pool that runs as the user "test-ssh" and group "clp."
   - Configure NGINX to use this PHP-FPM pool in its virtual host configuration.

7. PHPMyAdmin:
   - Install and configure PHPMyAdmin for managing the MySQL database.

8. HTTP to HTTPS Redirection:
   - Set up NGINX to redirect HTTP traffic to HTTPS for secure communication.
   - Configure Magento to use HTTPS for all store URLs.
   - Create and configure a self-signed SSL certificate for encryption.

9. Varnish Integration:
   - Install Varnish and configure it to work with Magento for caching and performance improvement.

In summary, this assignment involves setting up a web server environment with various software components, creating necessary users and groups, configuring each component for specific tasks, and ensuring secure and optimized operation for hosting Magento 2 with sample data.
