# Authentication

Flare currently requires the use of the Eloquent authentication driver to 
restrict access to the admin panel to authenticated users.

## Admin Authentication

By default Flare uses the built in Laravel authentication driver, Eloquent, to
provide authentication of the Flare admin panel. This means that all users
(defined by the authentication model records)  will have access to the admin
until you define an implicit set of access rules.

## Restricting Access to the Admin Panel




