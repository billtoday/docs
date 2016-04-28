# bts (npm module)

The bts module is the heart of the billtoday software stack. It allows you to easily manage payments and react to them within your apps.

For detailed usage information please read the [module's README](https://www.npmjs.com/package/bts)!

### What does the `bts` module do?
The bts module reads your config files and starts a bts instance. All transaction data is stored in a mongo database. When you upgrade bts the data in the database can persist. Any needed updates will be performed in place. You can specify a backup option to prevent data loss. But we recommend tools like [MongoDB Cloud Manager](https://www.mongodb.com/cloud/) for fine grained background backups.

#### It works with docker (Yeah!!!)

