# Kickstart troubleshooting use cases

## Unknown install type (F050C)

Uknown install type is a Netdata Agent deployment that we can be certain how it was installed. To that end,
we dont attempt to make any automated/scripted changes for not affect your system adversely. 

### Which type of Netdata deployments are charecterized as "Unknown"

In a nutshel whatever package/binary/deployment that was not shiped by the Netdata org. This category includes:

- Native packages shipped by community repos.
- Custom docker files (from private forks)

### Troubleshoot

#### Native deployments from open source package maintainers. 

In cases likes these we can't guarantee that everything will work as expected or that the integrations with other
Netdata products (such as the Netdata Cloud) will be seamless. If you choose to receive the Netdata Agent from 
your upstream distribution platform, you need to disable any autoupdate feature of the Netdata Agent (for 
instance from the cron scheduler) and rely on your package manager (manual or automated updates).

Otherwise you need to remove the packages installed (via your package manager) and follow our [official instructions](https://learn.netdata.cloud/docs/install-the-netdata-agent/) to deploy the Agent.

