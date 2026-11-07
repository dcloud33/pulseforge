# PulseForge

## Business Problem
- Application releases can introduce elevated HTTP 5xx error rates and increased request latency, negatively affecting customer experience and service reliability.
- Having to manually investigate the safety of a deployment, along with rollback decisions being inconsistent, due to release health isn't evaluated against defined criteria.
- Kubernetes reports that Pods are running, however customers are experincing failures.


## Project Objective
PulseForge aims to assess deployment health using predefined reliability criteria, including HTTP error rates, request latency, and application availability, to support evidence-based rollout and rollback decisions.

Measureable reliability signals:
- HTTP 5xx error rate
- Application availibility

## Initial Architecture
Provisioned the pulseforge-dev Namespace within the existing Docker Desktop Kubernetes cluster to provide a dedicated logical scope for project workloads.