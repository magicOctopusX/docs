# Manual cleaning an instance from the previous deployment

In order to delete build artifacts anyone can run `./rel/commands/clear_build.sh` from the root project directory. It will delete these folders:

* delete `_build` & `deps` directories
* delete node modules located at
* `apps/block_scout_web/assets/node_modules`
* & `apps/explorer/node_modules`
* delete `logs/dev` directory

{% hint style="info" %}
If it is required to delete static assets too \(`apps/block_scout_web/priv/static` folder\), for instance, before rebuilding to apply changes to front-end, anyone should run the previous command with `-f` flag:

`./rel/commands/clear_build.sh -f`
{% endhint %}

