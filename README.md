# D8ConfigBase
This is a config base for D8+ that will get most things going and provide much boiler plate.

## Usage
Download the zip of this and put it in to the sync dir of your "FRESH" D8 install.

Then change the site uuid in the file:

```
system.site.yml
```

If you are using the Content and Coffee DupalBase then your config dir will be in the directory:

```
config/sync
```

Use this command to get your current site uuid.

Ex,
```
> ../vendor/drush/drush/drush config-get "system.site" uuid
'system.site:uuid': ea80dc18-ae20-4b57-bb7d-6090b2b8a957
```

Then to import the configuration in this repo run this command.

```
../vendor/drush/drush/drush cim -y
```

Now the config will be installed in your fresh D8 and you will have some really good basics in order.

