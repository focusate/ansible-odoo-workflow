# Ansible playbooks/roles to Manage Odoo instances

You can use these playbooks to manage production and stage environments:

* Initially setup on freshly installed environment (needs root access):
    * install `docker`, `docker-compose`.
    * setup `odoo` user.
    * setup certificates for `nginx`.
    * automatically set admin password after Odoo instance is created.
    * set up an access between `prod` and `stage` common environments (e.g. Client A prod and stage environments).
    * configure PostgreSQL params (for tuning it).
* Backup (and rotate) database before updating.
* Restore prod backup on stage environment.
* Setup Odoo container combined with nginx and PostgreSQL
* Update Odoo container to take new changes.
