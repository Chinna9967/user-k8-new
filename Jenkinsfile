@Library('roboshop-shared-library') _

def configMap = [
    application: "nodeJSEKS",
    component: "user"
]

if (!env.BRANCH_NAME.equalsIgnoreCase("master")) {
    pipelineDecission.decidePipeline(configMap)
} else {
    echo "master deployment should happen through cr only"
}
