# spot-usage-for-kubernetes

How to balance cost and stability with spot in kubernetes.

This repository is created to provide sample implementation of ideas espoused in blog - [How to use Spot to achieve Cost Savings with Stability on Kubernetes](https://devtron.ai/blog/how-to-use-spot-to-achieve-cost-savings-on-kubernetes/)

This repository has three directories - **attempt_1**, **attempt_2**, **attempt_3**

- **attempt_1** : This is a **failed approach** in which we have ensured that node are in the required spot to on-demand ratio and assume that pod will distribute in the same ratio.

- **attempt_2** : This again is a **failed approach** which uses preferred node affinity to distribute the pods.

- **attempt_3** : This is final and **successful attempt** in this we have used concept introduced in kubernetes version 1.16 and made beta in 1.18. Pod Topology Spread Constraint to distribute pod between spot and on-demand instances in desired ratio.
