# SD3 Configurator [![Codacy Badge](https://api.codacy.com/project/badge/Grade/6907513e49be41b3baaf93c03cca8372)](https://www.codacy.com?utm_source=git@bitbucket.org&amp;utm_medium=referral&amp;utm_content=pramata/sd3_configurator&amp;utm_campaign=Badge_Grade)[![Codacy Badge](https://api.codacy.com/project/badge/Coverage/6907513e49be41b3baaf93c03cca8372)](https://www.codacy.com?utm_source=git@bitbucket.org&utm_medium=referral&utm_content=pramata/sd3_configurator&utm_campaign=Badge_Coverage)

## Description

This is the service that enables setting up new tenants for the SD3 platform and all configurations related to a tenant.
For any of the services listed below to work, this should be set up first.
-   SD3_ui

## Version Details

| Field                                 | Details                                  |
|:--------------------------------------|-----------------------------------------:|
| Ruby version                          | 2.4.2                                    |
| Rails version                         | 5.2.0                                    |

## Dependency List

### System Libraries

None

### Other Services

All the services specified here are required to set up a working tenant

| Name                            |               Description                                  |
|:--------------------------------|-----------------------------------------------------------:|
| S3                              | Amazon S3 file storage service                             |

## Setup Instructions

-   First time db set up : download the repo and run 

```
rake db:create && rake db:schema:load
```

-   with rails 5.2, SECRET_KEY_BASE should be made available in environment variable.
-   you can generate one by running *rake secret*

```
export SECRET_KEY_BASE="---secret key-----"
```
