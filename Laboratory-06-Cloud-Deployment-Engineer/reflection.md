# Mission Reflection

Completing Laboratory 06 helped me understand how Docker Compose makes cloud deployment easier and more organized. Instead of manually creating and configuring every container, I can define the services in a single `docker-compose.yml` file. This makes the deployment process more consistent, repeatable, and easier to manage. If I need to deploy the same application again, I can reuse the configuration instead of remembering every command and setting.

I also learned that YAML indentation is very important. Using the wrong number of spaces or pressing Tab instead of using spaces can cause a parsing error or place a configuration option under the wrong section. Because of this, I need to check the file carefully before deploying the application. Correct indentation helps Docker Compose understand the relationship between services, images, ports, and environment variables.

Environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` provide the configuration that Nextcloud and MariaDB need to communicate. They make it possible to configure the application without placing these settings directly in the application code. However, passwords written directly in a Compose file are not ideal for production because they can be exposed if the file is shared publicly.

Deploying Nextcloud with MariaDB was an exciting experience because it showed me how a private cloud storage system can be created within a few minutes. I understood that the web application and database have different responsibilities but must communicate to provide a working service. I also learned the importance of checking container status, viewing logs, and cleaning up resources after testing.

Since Mission 1, my understanding of cloud computing has developed from learning individual concepts and running separate containers to managing a complete application stack. I now understand that cloud engineers can use Infrastructure as Code to make deployments more efficient, consistent, and maintainable. This laboratory improved my confidence in using Linux commands, Docker Compose, and GitHub documentation for future cloud projects.
