# Deploy Lightstep Satellite On Render

[Lightstep Satellites](https://docs.lightstep.com/docs/learn-about-satellites) collect 100% of data that instrumented clients and servers emit and use it to assemble traces and compute an aggregate picture of spans.
Use the button below to deploy a Lightstep satellite as a [private service](https://render.com/docs/private-services) on render.

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

## Post Deploy
1. Login/Signup for a [Lightstep account](https://app.lightstep.com/) to get your own `COLLECTOR_SATELLITE_KEY`
  * Set this value in the dashboard directly.

2. Be sure to replace the following environment variables in `render.yml` with values suited for your use-case.
* COLLECTOR_POOL
* COLLECTOR_GUID
* COLLECTOR_BYTES_PER_PROJECT

See Lightstep's documentation to learn more about [recommended configurations](https://docs.lightstep.com/docs/satellite-configuration-parameters) for a collector.

### Deployment Issues

Lightstep has a [handy guide](https://docs.lightstep.com/docs/verify-satellite-setup) for verifying Satellites are setup correctly
