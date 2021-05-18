# Ansible and Terraform: Friendship is Magic

## Overview

This repository contains all the bits for driving Terraform using Ansible and Tower:

- `./rhel_config.yaml` is an Ansible playbook for basic RHEL configuration
- `./terraform` contains basic Terraform code for deploying a VMware instance
- `./terraform.yaml` is an Ansible playbook for wrapping Terraform

## Usage

## Making this Production Ready

Ideally, the Terraform wrapper would be an Ansible module you provide to your customers.  They would include the wrapper, update a few variables such as the location of the Terraform code (the `project_path` argument for the Terraform module accepts any path, including git).
