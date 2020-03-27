# Deploy Lightstep Collector On Render

Use the button below to deploy a [Lightstep collector](https://docs.lightstep.com/docs/install-and-configure-satellites) as a [private service](https://render.com/docs/private-services) on render.

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy)

## Post Deploy
1. Login/Signup for a [Lightstep account](https://app.lightstep.com/) to get your own `COLLECTOR_SATELLITE_KEY`
  * Set this value in the dashboard directly.

2. Be sure to replace the following environment variables in `render.yml` with values suited for your use-case. 
* COLLECTOR_POOL 
* COLLECTOR_GUID
* COLLECTOR_BYTES_PER_PROJECT

See lightstep's documentation to learn more about [recommended configurations](https://docs.lightstep.com/docs/satellite-configuration-parameters) for a collector.
