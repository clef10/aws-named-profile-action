# AWS named profile for Github Action
Written this custom action for a use-case in the org, it is compact and have helped a lot. Feel free to use if you get the requirement.
## Overview
It is built on top of aws-actions/configure-aws-credentials and is a simple action that generates the named profile with aws cli.

Kindly use the following config for this action:
```
- name: Setup AWS named profile
  uses: clef10/aws-named-profile-action@v1.0.0
  with:
    role-to-assume: arn:aws:iam::123456789100:role/my-github-actions-role
    profile: default
    region: us-east-2
```
## References
- [aws-actions/configure-aws-credentials@v4](https://github.com/aws-actions/configure-aws-credentials)
