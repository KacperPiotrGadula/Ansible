# Basic Structure of Ansible Folder Structure

## Files

This directory contains files that will be copied to target machines by the copy or template modules. Typically, it holds binary files, scripts, configurations, etc., used during task execution.

## Handlers

Handlers are tasks triggered in response to specific events during playbook execution. They are commonly used for restarting services or performing other actions in response to changes.

## Meta

The meta directory may contain metadata related to the role, such as dependencies, author, license, etc. This directory is optional.

## Tasks

This directory contains YAML files defining a list of tasks to be executed on target machines. These are the basic Ansible instructions that specify what the role or playbook should accomplish.

## Templates

The templates directory holds template files that are rendered on target machines before use. Templates may contain variables, loops, conditions, and other Ansible template language constructs.

## Vars

The vars directory contains YAML files containing variables that can be used in playbooks or roles. These variables can be global to the role or specific to particular tasks.