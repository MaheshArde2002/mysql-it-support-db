# MySQL Security Configuration

## Objective

Perform basic security configuration of the MySQL Server using `mysql_secure_installation`.

## 1. Run mysql_secure_installation

Run the following command:

```bash
mysql_secure_installation

This command provides basic security configuration options for MySQL.

2. Root Authentication

During the configuration, MySQL displayed:

Skipping password set for root as authentication with auth_socket is used by default.

This means the MySQL root account is using auth_socket authentication.

A root password was not set through this process.

3. Remove Anonymous Users

MySQL asks:

Remove anonymous users?

Select:

y

The anonymous users are then removed.

4. Security Configuration

The mysql_secure_installation command can be used for basic MySQL security configuration, including:

Removing anonymous users
Configuring root authentication
Removing unnecessary test settings
Applying basic security settings

In this project:

Anonymous users were removed.
MySQL root authentication continued to use auth_socket.
A root password was not configured through mysql_secure_installation.
Result

Basic MySQL security configuration was completed successfully.

