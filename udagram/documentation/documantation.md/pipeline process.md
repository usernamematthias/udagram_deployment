
# Pipeline Process

see `00_pipeline overview` picture in `pipeline` folder

1. Every committed change to `GITHUB` is transferred to circleCI and initiates the pipeline workflow
2. Orbs are defined in the `config.yml` in the `.circleci` folder; they contain basic recipes and reproducible actions 
    1. install node
    2. set up AWS 
    3. and set up elastic beanstalk

3. The code from the `GITHUB` repo will be testet in the defined jobs:
* install dependencies (front end and back end cf. `picture 00_pipeline overview`)
* build
* deploy

4. App available for user at AWS
