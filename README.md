# docker-chef
Developer environment for using chef, notably being able to run `kitchen converge` on Windows without pulling your hair out. Currently only works when using `docker` driver.

## Installation
- Clone the repo
- Clone any chef repositories you want to work with in inside the `projects` directory
    - Add `use_internal_docker_network: true` under the `driver` section in your `kitchen.yml` for those projects

## Usage

- Run `docker-compose run chefdk bash` from the root of this repository
- Navigate to your project and run `kitchen converge`