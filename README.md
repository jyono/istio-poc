# istio-poc


## Requirements

### Docker
https://docs.docker.com/get-docker/

### kubectl
https://kubernetes.io/docs/tasks/tools/

### minikube
install minikube https://minikube.sigs.k8s.io/docs/start/

### bazel
https://docs.bazel.build/versions/4.2.1/tutorial/java.html
https://docs.bazel.build/versions/main/tutorial/java.html

build with
`bazel build //:ProjectRunner --javabase=@bazel_tools//tools/jdk:remote_jdk11`

run with
`bazel-bin/ProjectRunner`

dep-graph with 
`bazel query  --notool_deps --noimplicit_deps "deps(//:ProjectRunner)" --output graph`

