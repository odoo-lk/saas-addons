[![Build Status](https://travis-ci.com/it-projects-llc/saas-addons.svg?branch=17.0)](https://travis-ci.com/it-projects-llc/saas-addons)

# SaaS addons

System to sale and manage odoo databases.

The repository contains modules for master instance (old name: *SaaS Portal*). Other resources of the project:

* https://saas.it-projects.info -- main website
* https://gitlab.com/itpp/saas-clusters -- modules for multi-server deployment
* https://github.com/itpp-labs/access-addons -- useful modules for client instances (*SaaS Client*)
* https://github.com/it-projects-llc/odoo-saas-tools -- abandoned original repository

## Odoo 17.0 Upgrade

This repository has been upgraded for Odoo 17.0 compatibility. Key changes made:

- All module versions updated from 15.0.x.x.x to 17.0.x.x.x format
- Deprecated `web.assets_qweb` replaced with `web.assets_web` in manifest files
- Empty `qweb` keys removed from manifest files (deprecated in Odoo 17.0)
- Python 3.8+ now required (updated in CI configuration)

**Migration notes:**
- Module loading should work without changes for most modules
- JavaScript assets using legacy `web.*` imports may work through backward compatibility, but should be monitored for deprecation warnings
- All manifest files follow Odoo 17.0 standards
