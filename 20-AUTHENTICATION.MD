# Authentication

## Admin Authentication
The default configuration of Flare uses the built in Laravel Authentication Driver to provide the authentication of tbe Falre Admin panel. This means that all users who have accounts associated with the Auth Model (defined in your `config/auth.php`) will have access to the administration panel until you define an implicit set of access rules.

Flare allows you to define a custom Permissions Provider to control overall access to your administration panel and also provides the opportunity to provide custom Policies to sections of thr admin panel and any available actions.
