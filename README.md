# Composer WordPress Skeleton

This is simply a skeleton repo for a WordPress site, forked from [ADARTA](https://github.com/ADARTA/Composer-Wordpress-Skeleton/) and modified to my needs. Read the original README and use with caution.

## Short guide:
1. Clone this git into `htdocs`:  
`git clone git@github.com:moritzjacobs/Composer-Wordpress-Skeleton.git my-server-root`
2. Edit `wp-config-local-sample.php` and enter valid db credentials
3. `composer install`
4. Surf to localhost

### Differences to ADARTA's version:

* Removed roots support
* Renamed `wp-content/` to `site/` and `wp/` to `core/`
* What is `web.config`? I don't know eiter, be gone.
* `wp-config-*.php` support with auto-switching by host name (`local | staging | live`)
* Plugin activation is handled by `mu-plugins/plugin-bootstrap.php`; Plugins are inactive if their root folder/file name starts with an underscore
* Read .gitignore to get an idea about what we're trying to accomplish with git and composer here