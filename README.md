# GitOps-starter

1. `mv .banzai-example .banzai`
2. Update the `envs/` directory. There should be a sub-folder for each environment you wish to maintain ie) `envs/dev/` or `envs/qa/`
3. Add a stack.yaml to each newly created env directory. ie) `envs/dev/mystack.yaml`
    - The stack.yaml file can be empty OR can contain key-value pairs formatted `<service-id>: '<service-version>'`
4. Update the `services/` directory. The services directory should contain a .yaml file for each service you would like to have deployed to a stack. If a service triggers a GitOps build and a file does not exist. One will be created automatically.
5. Update the .banzai to fit your use-case