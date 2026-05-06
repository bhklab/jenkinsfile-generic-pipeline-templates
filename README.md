# jenkinsfile-generic-pipeline-templates

This repository contains reusable Jenkins pipeline templates for data workflows, with a focus on Kubernetes-based execution and Snakemake pipelines run via Pixi + Conda.

## Included templates

- `Jenkinsfile.pixi-snakemake` - a generic Jenkins pipeline that:
  - launches a Kubernetes pod with a Pixi/Snakemake execution container
  - checks out a repository branch
  - installs the Pixi environment
  - performs a Snakemake dry run and actual run
  - uploads pipeline results to Google Cloud Storage

## Purpose

Use these templates as a starting point for building Jenkins pipelines that run scientific or bioinformatics workflows inside containerized Kubernetes agents.

## Notes

- This repo is intended for pipeline template sharing and reuse across multiple projects.
