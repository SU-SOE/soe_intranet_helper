#[Stanford Intranet helper](https://github.com/SU-SWS/soe_intranet_helper)
##### Version: 7.x-1.x

Maintainers: [cjwest](https://github.com/cjwest), [boznik](https://github.com/boznik)
[Changelog.txt](CHANGELOG.txt)

The SoE Intranet Helper is for customizations for the 
[SoE Intranet site](https://sites.stanford.edu/jse-soe-intranet). Specifically it:
 - Assists when the standard Drupal caching may be incomplete. This implements a function to look for a sidebar on a page with a node. If it is not there, flush the cache.

Installation
---

Install this module like any other module. [See Drupal Documentation](https://drupal.org/documentation/install/modules-themes/modules-7)

Configuration
---

Nothing special needed.

Troubleshooting
---

If you are experiencing issues with this module try reverting the feature first. If you are still experiencing issues try posting an issue on the GitHub issues page.
To verify configuration:

To verify that the `soe_intranet_helper_settings` are set:
```
drush vget soe_intranet_helper_settings
soe_intranet_helper_settings:
whitelist:
  :
  ```

To verify in the logs or (`drush ws --tail`) you see something like:

```debug soe_intranet_helper First sidebar is missing. Page is: node/xxx```

Contribution / Collaboration
---

You are welcome to contribute functionality, bug fixes, or documentation to this module. If you would like to suggest a fix or new functionality you may add a new issue to the GitHub issue queue or you may fork this repository and submit a pull request. For more help please see [GitHub's article on fork, branch, and pull requests](https://help.github.com/articles/using-pull-requests)
