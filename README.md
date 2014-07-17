# Composer WordPress Skeleton

This is simply a skeleton repo for a WordPress site, forked from [ADARTA](https://github.com/ADARTA/Composer-Wordpress-Skeleton/) and modified to my needs. Read the original README and use with caution.

## Short guide:
1. Clone this git into `htdocs`:  
`git clone git@github.com:moritzjacobs/Composer-Wordpress-Skeleton.git my-server-root`
2. Edit `wp-config-local-sample.php` and enter valid db credentials, then rename to `wp-config-local.php`
3. Change the Wordpress table prefix in `wp-config.php` (line 52)
4. `composer install`
5. Surf to `http://mycrazyhostname.dev/admin`
6. Follow install process
7. Update Wordpress via the Dashboard (why you need to do this, I have *no* idea...)


### Differences to ADARTA's version:

* Removed roots
* Renamed `wp-content/` to `site/` and `wp/` to `core/`
* Removed `web.config`
* `wp-config-*.php` support with auto-switching by host name (`local | staging | live`)
* Plugin activation is handled by `mu-plugins/plugin-bootstrap.php`; Plugins are inactive if their root folder/file name starts with an underscore
* Read .gitignore to get an idea about what we're trying to accomplish with git and composer here