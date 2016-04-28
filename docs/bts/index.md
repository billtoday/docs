# bts (npm module)

The bts module is the heart of the billtoday software stack. It allows you to easily manage payments and react to them within your apps.

For detailed usage information please read the [module's README](https://www.npmjs.com/package/bts)!

### What does the `bts` module do?
The bts module reads your config files and starts a bts instance. All transaction data is stored in a mongo database. When you upgrade bts the data in the database can persist. Any needed updates will be performed in place. You can specify a backup option to prevent data loss. But we recommend tools like [MongoDB Cloud Manager](https://www.mongodb.com/cloud/) for fine grained background backups.

#### Docker
We recommend using bts with docker. It is the easiest and fastest to upgrade and maintain.
You can get the official [ht-docker-billtoday](https://hub.docker.com/r/hosttoday/ht-docker-billtoday/) container on docker hub. It includes bts and a test database for demo purposes. For production you can specify MongoDB credentials via an ENV var at the first run.

The ht-docker-billtoday container is host.today compliant. This means you can use it with the [ht-docker-traffic](https://hub.docker.com/r/hosttoday/ht-docker-traffic/) container.

