# UdacityDevOpsThirdProject
[![frenandi](https://circleci.com/gh/frenandi/UdacityDevOpsThirdProject.svg?style=svg)](https://github.com/frenandi/UdacityDevOpsThirdProject)

## Summary

In this project, one Machine Learning API to make predictions was deployed using Docker and Kubernetes. Also CircleCI was used for continues integration where Hadolint and Pylint were used to validate Dockerfile and the python application.

The following tasks were performed in order to complete the project.

1. Configure CircleCI environment.
2. Create and activate a Python environment.
3. Manually Run Lint checks.
4. Install Minikube to run Kubernetes cluster locally.
5. Complete Dockerfile to deploy container containing the Python app.
6. Improve Logging for the Python app.
7. Upload the Docker image to Docker Hub.
8. Configure Kubernetes to run locally.
9. Deploy app with Kubernetes.
10. Integrate with CircleCI.

---

## Instructions to run Python script

* Create a virtualenv and activate it
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

---

## Files Included

1. .circleci: contains the configuration file to perform the continues integration task using CircleCI tool.
2. output_txt_files: contains two files
  a. docker_out.txt: contains the output from the prediction output when the Docker container was running.
  b. kubernetes_out.txt: contains the output from the prediction output whe the Kubernetes cluster was running.
3. app.py: contains the script to make the predictions.
4. Dockerfile: contains the information to build the Docker container for the prediction app.
5. Makefile: contains a set of insturction to install requirements and lint operations.
6. requirements.txt: contains the information of all the libraries required by the app.
7. run_docker.sh: contains the instructions to create Docker container.
8. upload_docker.sh: contains the instructions to upload the Docker image to DockerHub
9. run_kubernetes.sh: conatins the instructions to set the Kubernetes cluster.
