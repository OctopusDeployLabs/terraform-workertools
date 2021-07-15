FROM octopuslabs/workertools:latest-ubuntu.2004

ARG DEBIAN_FRONTEND noninteractive

# Get Terraform
# https://computingforgeeks.com/how-to-install-terraform-on-ubuntu-centos-7/
RUN curl -fsSL https://apt.releases.hashicorp.com/gpg | apt-key add - && \
    apt-add-repository "deb [arch=amd64] https://apt.releases.hashicorp.com $(lsb_release -cs) main" && \
    apt-get update && apt-get install terraform -y