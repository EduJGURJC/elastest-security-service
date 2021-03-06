# ElasTest Security Service (ESS)

The ElasTest Security Service (ESS) is an ElasTest service for identifying security issues in the System Under Test (SuT) by mimicking attacker behavior. Thus, when finding security issues, the focus is not in generating test cases that capture normal user behavior with the SuT. Instead, ESS focuses on generating test cases that check the SuT reaction to abnormal behavior (e.g. modifying URL parameters, using incorrect requests, or replaying authorization requests).

## Features
The final version of ESS is expected to support the detection of the following types of vulnerabilities/attacks:
1. Logical vulnerability
2. Denial-of-Service
3. Improper/Missing authentication

The current version of ESS (v0.1) has the following features.

- Create a secJob from a tJob
- Update and Delete secJobs
- Execute a tJob associated to the secJob
- Show the mockup of the creation of a malicious tJob that exposes a replay attack vulnerability in TomatoCart (an open source e-commerce web application)

## How to run

ESS can be installed by running the following documentation provided [here](https://docs.google.com/document/d/1bKEMpXKUAaE0Re7hNxCKY99D6HSuy96cwqZ5rQkEERs/edit?usp=sharing).

## Basic usage

When ElasTest ESS is started, its API is accessible in the following URL:
- Linux & Windows: http://localhost:80/
The API description is [available](http://elastest.io/docs/api/ess/).

## Development documentation

### Architecture

ESS is implemented in two parts:
* ESS Web client Application: A web-based GUI for interacting with the ESS API
* ESS Server Application: The back-end of the ESS API
