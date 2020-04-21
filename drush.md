Migrate command
```
drush ms
drush migrate:import <migration name>
drush migrate:reset-status <migration name>
drush migration:rollback <migration name>
```

```
drush migrate-reset-status <MIGNAME>
drush pm-uninstall <MIGMODULENAME>
drush pm-install <MIGMODULENAME>
```

Config command
```
drush config-split-export
drush config-split:export
drush config-split-import
drush config-split-export <dev>
drush config-split-import <sync>
drush config-split:import config_dev

drush cim
drush cex

drush cex --no
drush cex --no | grep -q identical
```

```
drush config-status or drush config:status
drush config:status --state="Only in DB"
drush config:status --prefix="image"
drush config-list
drush config-list views

drush config-get <config-name>
drush config-set <config-name> <config-key> <value>
drush config-set system.site name "Configuration Management with Drush"
drush config-edit <config-name>
```

To look at system.site configuration
```
drush cget system.site
```

Common command 
```
drush cr
```

