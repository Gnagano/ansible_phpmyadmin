# Ansible Role: install phpmyadmin and set up for nginx

---

## Requirements

OS: Ubuntu16.04
`php` and `nginx` is installed before this.

## Getting started

```
$ ansible_galaxy install gano2018.ansible_phpmyadmin --roles-path <your_roles_directory>
```

## Role Variables you need to edit

- phpmyadmin_link_dir

  This variable is the directory where phpmyadmin will be linked. Usually this is document root for nginx.
  The default value is `/home/doc_root`

- phpmyadmin_link_name:

  This variable is the name of access path to phpmyadmin.
  If you set the value `phpmyadmin`, you can access to phpmyadmin by browser, the url `http://server_name/phpmyadmin.`
  Changing the name `phpmyadmin` is recommended because of the security reason.
