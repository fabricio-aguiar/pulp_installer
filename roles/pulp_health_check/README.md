pulp_health_check
=================

Verify pulp healthy.

Role Variables
--------------

* `pulp_admin_username`: The pulp admin username. Defaults to `admin`.
* `pulp_validate_certs`: Control if the SSL certificate from the Pulp server should be validated
   or not. Defaults to `yes`.


Shared Variables
----------------

This role is **not tightly coupled** to the `pulp_common` role, but uses some of the same
variables. When used in the same play, the values are inherited from the role.
When not used together, this role provides identical defaults.

* `pulp_default_admin_password`: Initial password for the Pulp admin. **Required**.
* `pulp_api_bind`: Set the host the reverse proxy should connect to for the API server. Defaults
  to '127.0.0.1:24817'.

Operating Systems Variables
---------------------------

Each currently supported operating system has a matching file in the "vars"
directory.
