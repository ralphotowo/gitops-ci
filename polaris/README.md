The custom config file needs to be baked into the docker image and used as follows:


polaris  audit -c polaris/polaris-check.yaml --audit-path . --format=pretty --only-show-failed-tests true --set-exit-code-below-score 99
