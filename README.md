# Muryoutaisuu's Notes on CNCF & KubeCon 2019, Barcelona

Notes, links etc. by me, Natalie Fioretti

[All available presentation slides](https://kccnceu19.sched.com/list/descriptions/)

[Youtube Playlist with all available presentation videos](https://www.youtube.com/playlist?list=PLj6h78yzYM2PpmMAnvpvsnR4c27wJePh3)
## Lightning Talks, 20.05.2019

#### Beyond Operators: Reimagine Distributed Applications on Kubernetes

- k8s is a platform for building platforms, it's not the end! -> **k8s Controllers/Operators**
- These are a good beginning, but go beyond it! -> Coordinator/worker principle
- Still a POC, might become popular in future, because it leverages the API knowledge of developers

#### Kubernetes Jobs and the Sidecar Problem

- Sidecar containers will run indefinitely, even if the main containers was completed/failed (if you only scheduled jobs)
- *If you have a Job with two containers one of which is actually doing the main processing of the job and the other is just facilitating it, you encounter a problem when the main process finishes; your sidecar container will carry on running so the job will never finish.* [[source](https://github.com/kubernetes/enhancements/blob/master/keps/sig-apps/sidecarcontainers.md#jobs)]
- [presentation](https://static.sched.com/hosted_files/kccnceu19/9d/Kubernetes%20Jobs%20and%20the%20Sidecar%20Problem%20Lightning%20Talk%20-%20James%20Wen%2C%20Spotify.pdf)

#### 

## Keynotes

#### Keynotes 100, 21.05.2019

- openebs, container attached storage
- linkerd: service mesh observability, security etc.,
- rook: production ready block storage
- cri-o: another k8s container engines, only engine for oshift4.1+
- opencensus+opentracing: opentelemetry combines bove (with backwardscompability bridges)
- fluentd: unified logging layer, new documentation, faster performanter with tls in syslog and http
- cisco: network service mesh, access complicated L2/L3 k8s services, ignore vlan, routing, etc.
## Sessions

### sessionname
## Keywords

#### ebpf
- routing, tracing
- [slides](https://static.sched.com/hosted_files/kccnceu19/b8/KubeCon-Europe-2019-Beatriz_Martinez_eBPF.pdf)
- [introduction to ebpf](https://www.redhat.com/en/blog/introduction-ebpf-red-hat-enterprise-linux-7)

#### kubespray
- deploy k8s clusters
- [github repository](https://github.com/kubernetes-sigs/kubespray)

#### service mesh
- [What's a service mesh, and do I need it?](https://github.com/kubernetes-sigs/kubespray)
- e.g. linkerd