## Lightning Talks, 20.05.2019

#### Beyond Operators: Reimagine Distributed Applications on Kubernetes

- k8s is a platform for building platforms, it's not the end! -> **k8s Controllers/Operators**
- These are a good beginning, but go beyond it! -> Coordinator/worker principle
- Still a POC, might become popular in future, because it leverages the API knowledge of developers

#### Kubernetes Jobs and the Sidecar Problem

- Sidecar containers will run indefinitely, even if the main containers was completed/failed
- *If you have a Job with two containers one of which is actually doing the main processing of the job and the other is just facilitating it, you encounter a problem when the main process finishes; your sidecar container will carry on running so the job will never finish.* - https://github.com/kubernetes/enhancements/blob/master/keps/sig-apps/sidecarcontainers.md#jobs

- presentation: https://static.sched.com/hosted_files/kccnceu19/9d/Kubernetes%20Jobs%20and%20the%20Sidecar%20Problem%20Lightning%20Talk%20-%20James%20Wen%2C%20Spotify.pdf
