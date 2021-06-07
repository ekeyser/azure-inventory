azure-inventory
========

#### Azure Infrastructure Inventory ####

This module provides an abstraction layer to inventory your cloud resources.

Supported services (and APIs):

Supported Regions
`us-west-1`

### Installation ###
```bash
npm install azure-inventory
```

### Usage ###

```javascript
import AzureInventory from 'azure-inventory'

const config = {
  credentials: {
    accessKeyId: 'your_access_key',
    secretAccessKey: 'your_secret_key'
  },
  services: ['ec2', 'rds'],
  regions: ['us-west-2, us-east-1']
};

const oInventory = new AzureInventory(config);
const oResources = oInventory.inventory();
```
