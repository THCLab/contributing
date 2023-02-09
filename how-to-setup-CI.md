# CI templates

### WASM bindings (check [THCLab/oca-rs](https://github.com/THCLab/oca-rs) for reference)

- [Template](./templates/wasm) for building web and nodejs package

## Github Actions

### Docker Hub

- [Build and push image](./templates/workflows/docker-publish.yml)  
_Repository secrets_:
  - `DOCKERHUB_USERNAME`
  - [`DOCKERHUB_TOKEN`](https://docs.docker.com/docker-hub/access-tokens/)

### Rust

- [Basic code checks](./templates/workflows/rust/basic.yml)
- [Publish to crates.io](./templates/workflows/rust/publish.yml)  
_Repository secrets_:
  - [`CARGO_REGISTRY_TOKEN`](https://crates.io/settings/tokens)

#### WASM bindings (check [THCLab/oca-rs](https://github.com/THCLab/oca-rs) for reference)

- [Build and check package](./templates/workflows/rust/wasm.yml)
- [Publish to npmjs.com](./templates/workflows/rust/wasm-publish.yml)  
_Repository secrets_:
  - [`NPM_TOKEN`](https://docs.npmjs.com/creating-and-viewing-access-tokens)

### JavaScript / TypeScript

- [Publish to npmjs.com](./templates/workflows/javascript/publish.yml)  
_Repository secrets_:
  - [`NPM_TOKEN`](https://docs.npmjs.com/creating-and-viewing-access-tokens)
