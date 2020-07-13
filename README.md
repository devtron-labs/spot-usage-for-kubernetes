# spot-usage-for-kubernetes

How to balance cost and stability with spot in kubernetes.

This repository is created to provide sample implementation of ideas espoused in blog ...

This repository has three directories - **Attempt 1**, **Attempt 2**, **Attempt 3**

- **Attempt 1** : This is a **failed approach** in which we have ensured that node are in the required spot to on-demand ratio and assume that pod will distribute in the same ratio.

- **Attempt 2** : This again is a **failed approach** which uses preferred node affinity to distribute the pods.

- **Attempt 3** : This is final and **successful attempt** in this we have used concept introduced in kubernetes version 1.16 and made beta in 1.18. Pod Topology Spread Constraint to distribute pod between spot and on-demand instances in desired ratio.
