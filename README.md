# README

Exploration of Synology NAS Web APIs. The aim is to be able to automate management initially of images and VMs, later of Docker images and containers.

The Synology Web API documentation is not straightforward to follow. The higher level abstractions in terraform providers and in Python APIs do not yet seem mature for these use cases. Initially understanding repeatable actions at the API level will help with making the higher level scenarios work.

## Setup

### REST Client

The API discovery is based on using the [REST Client](https://marketplace.visualstudio.com/items?itemName=humao.rest-client) Visual Studio Code extension.

### Environment Variables

Create a `.env` file in the project directory and populate with the following environment variables, populated with appropriate values.

```shell
SYNOLOGY_IP_ADDRESS=192.168.x.y
SYNOLOGY_PROTO=http
SYNOLOGY_PORT=5000
SYNOLOGY_USERNAME=user
SYNOLOGY_PASSWORD=password
```

## Issues

- Many endpoints to add here
- Create VM image not yet working

## References

- Python API [N4S4/synology-api](https://github.com/N4S4/synology-api)
- Terraform provider [synology-community/synology](https://registry.terraform.io/providers/synology-community/synology/latest/docs)
- [Synology Virtual Machine Manager API Guide](https://global.download.synology.com/download/Document/Software/DeveloperGuide/Package/Virtualization/All/enu/Synology_Virtual_Machine_Manager_API_Guide.pdf)