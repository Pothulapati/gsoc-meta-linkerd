# Google Summer of Code 2019 Internship with Linkerd

My GSoC work was aimed to contribute to the SMI-Metrics repository i.e to add support for Istio and also work on other Issues. As the SMI-Metrics project was pretty new, to keep up my work and not get struck on one thing, I also contributed to the Linkerd project i.e fixing issues, adding more features, etc.

## General Info

+ Name: Tarun Pothulapati
+ Github: [pothulapati](www.github.com/pothulapati)
+ Email: tarunpothulapati@outlook.com
+ Blog: www.tarunpothulapati.com
+ Mentor: Thomas Rampelberg

## Contributions to SMI-Metrics

Intially the SMI-Metrics, had a very hard dependency on prometheus for metrics as it was still a prototype. This can be a challenge for service mesh projects that don’t depend on prometheus for queries or had a drastically different structure of time-series (i.e labels, sum of multiple metrics,etc ). So, I worked on adding a Mesh Interface and de-coupling the prometheus client. This made the repo more extensiable i.e now service meshes can just implement the interface and reply those metrics with or without prometheus.

### Blog Posts

+ [SMI-Metrics with Istio](https://www.tarunpothulapati.com/posts/my-gsoc-journey-with-linkerd/)

*The above blog post consists of a demo of SMI-Metrics with Istio support that I worked on.*

### Design Docs

+ [Istio Support](https://docs.google.com/document/d/1mOlmwjLjoR1dus8G68ChYxJ_TJLBBvIdbYdGacFbeNM/edit?usp=sharing)

### Code Contributions

**Repository: smi-metrics**

Total Pull Requests Created: 14

1. [deislabs/smi-metrics#37](https://github.com/deislabs/smi-metrics/pull/37) - Move Queries struct to a common package.
2. [deislabs/smi-metrics#36](https://github.com/deislabs/smi-metrics/pull/36) - Single version Variable for both charts and  docker images
3. [deislabs/smi-metrics#31](https://github.com/deislabs/smi-metrics/pull/31) - Release automation through CircleCI
4. [deislabs/smi-metrics#30](https://github.com/deislabs/smi-metrics/pull/30) - smi metrics istio installation through helm
5. [deislabs/smi-metrics#25](https://github.com/deislabs/smi-metrics/pull/25) - Istio Support for SMI-Metrics
6. [deislabs/smi-metrics#23](https://github.com/deislabs/smi-metrics/pull/23) - Mesh Interface and Refactoring
7. [deislabs/smi-metrics#19](https://github.com/deislabs/smi-metrics/pull/19) - Fix unused dependencies using go mod tidy
8. [deislabs/smi-metrics#13](https://github.com/deislabs/smi-metrics/pull/13) - Add usage docs
9. [deislabs/smi-metrics#11](https://github.com/deislabs/smi-metrics/pull/11) - Added CircleCI Config
10. [deislabs/smi-metrics#7](https://github.com/deislabs/smi-metrics/pull/7) - Reading Queries from Config yaml
11. [deislabs/smi-metrics#5](https://github.com/deislabs/smi-metrics/pull/5) - Remove NetRC dependency as the repo's are public

Total Issues Opened: 11

1. [deislabs/smi-metrics#28](https://github.com/deislabs/smi-metrics/issues/28) - Add Tests for Istio pkg
2. [deislabs/smi-metrics#27](https://github.com/deislabs/smi-metrics/issues/27) - Update Istio docs with configuration options through helm
3. [deislabs/smi-metrics#26](https://github.com/deislabs/smi-metrics/issues/26) - Template response latency queries.
4. [deislabs/smi-metrics#24](https://github.com/deislabs/smi-metrics/issues/24) - Move prometheus related code out of linkerd
5. [deislabs/smi-metrics#22](https://github.com/deislabs/smi-metrics/issues/22) - Service shouldnt 404 on `/` endpoint
6. [deislabs/smi-metrics#20](https://github.com/deislabs/smi-metrics/issues/20) - Fix make build
7. [deislabs/smi-metrics#18](https://github.com/deislabs/smi-metrics/issues/18) - ApiService dosen't run on 1.15
8. [deislabs/smi-metrics#9](https://github.com/deislabs/smi-metrics/issues/9) - More documentation on the SMI APIService
9. [deislabs/smi-metrics#8](https://github.com/deislabs/smi-metrics/issues/8) - Negative Values in the latency metrics.
10. [deislabs/smi-metrics#4](https://github.com/deislabs/smi-metrics/issues/4) - Support Metrics from Istio
11. [deislabs/smi-metrics#3](https://github.com/deislabs/smi-metrics/issues/3) - Making Queries Configurable

Total Pull Requests Reviewed: 2

1. [deislabs/smi-metrics#35](https://github.com/deislabs/smi-metrics/pull/35) - Match circle's arcane filters pattern
2. [deislabs/smi-metrics#33](https://github.com/deislabs/smi-metrics/pull/33) - Update release tooling to trigger off a tag

## Contributions to Linkerd

Throughout the GSoC period, I also kept my contributions up to Linkerd solving issues ranging from small bug fixes to small scale features.

### Blog Posts

- [Traffic Splitting in Linkerd](https://www.tarunpothulapati.com/posts/traffic-splitting-linkerd/)

**Repository: linkerd2**
Total Pull Requests Created: 18

1. [linkerd/linkerd2#3194](https://github.com/linkerd/linkerd2/pull/3194) - Check for Namespace level config override annotations
2. [linkerd/linkerd2#3193](https://github.com/linkerd/linkerd2/pull/3193) - Setting SuccessfulJobHistoryLimit to 0 for CronJobs
3. [linkerd/linkerd2#3153](https://github.com/linkerd/linkerd2/pull/3153) - replace extensions/v1beta1 to apps/v1beta1
4. [linkerd/linkerd2#3152](https://github.com/linkerd/linkerd2/pull/3152) - Add Node Selectors to select only linux nodes
5. [linkerd/linkerd2#3092](https://github.com/linkerd/linkerd2/pull/3092) - Added Resource Limits when ha is Configured
6. [linkerd/linkerd2#3038](https://github.com/linkerd/linkerd2/pull/3038) - Fix inject with path and add tests
7. [linkerd/linkerd2#2988](https://github.com/linkerd/linkerd2/pull/2988) - linkerd inject from remote URL
8. [linkerd/linkerd2#2984](https://github.com/linkerd/linkerd2/pull/2984) - add admin port label to proxy-injector and sp-validator
9. [linkerd/linkerd2#2963](https://github.com/linkerd/linkerd2/pull/2963) - Add sideEffects field to Webhooks
10. [linkerd/linkerd2#2893](https://github.com/linkerd/linkerd2/pull/2893) - Added Anti Affinity when HA is configured
11. [linkerd/linkerd2#2874](https://github.com/linkerd/linkerd2/pull/2874) - HA for proxy-injector and sp-validator
12. [linkerd/linkerd2#2853](https://github.com/linkerd/linkerd2/pull/2853) - Added labels to webhook configurations in charts/
13. [linkerd/linkerd2#2820](https://github.com/linkerd/linkerd2/pull/2820) - Added controller component labels to webhook configurations
14. [linkerd/linkerd2#2439](https://github.com/linkerd/linkerd2/pull/2439) - Added Jobs Resource to Linkerd Dashboard along with grafana.
15. [linkerd/linkerd2#2416](https://github.com/linkerd/linkerd2/pull/2416) - WIP: Wire up stats and dashboards for Jobs
16. [linkerd/linkerd2#2387](https://github.com/linkerd/linkerd2/pull/2387) - WIP: Wire up stats and dashboards for Jobs
17. [linkerd/linkerd2#2293](https://github.com/linkerd/linkerd2/pull/2293) - Added ep Alias for endpoints command
18. [linkerd/linkerd2#2292](https://github.com/linkerd/linkerd2/pull/2292) - Ignoring resources with empty kind field.

Total Pull Requests Reviewed: 3

1. [linkerd/linkerd2#3266](https://github.com/linkerd/linkerd2/pull/3266) - Fix integration test
2. [linkerd/linkerd2#3039](https://github.com/linkerd/linkerd2/pull/3039) - Fix linkerd inject url handling
3. [linkerd/linkerd2#3032](https://github.com/linkerd/linkerd2/pull/3032) - Add release notes for stable-2.4.0

**Repository: rfc**

Total Pull Requests Created: 1

1. [linkerd/rfc#3](https://github.com/linkerd/rfc/pull/3) - Obsevarbility through GraphQL

## Conclusion

I had a great time working with the Linkerd team and especially Thomas (my mentor). I got the oppurtunity to work on latest cutting edge technologies like Kubernetes, etc.

More information on my Google Summer of Code experience can be found [here](https://www.tarunpothulapati.com/posts/my-gsoc-journey-with-linkerd/)
