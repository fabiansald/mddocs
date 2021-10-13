# OPENSHIFT ASSESSMENT - RACKSPACE

```
default/openshift:6443/admin
```

## OCP get nodes

### NODES

```
NAME                 STATUS   ROLES           AGE    VERSION           INTERNAL-IP      EXTERNAL-IP   OS-IMAGE                                                       KERNEL-VERSION                 CONTAINER-RUNTIME
crc-fd5nx-master-0   Ready    master,worker   440d   v1.18.3+012b3ec   192.168.126.11   <none>        Red Hat Enterprise Linux CoreOS 45.82.202007240629-0 (Ootpa)   4.18.0-193.13.2.el8_2.x86_64   cri-o://1.18.3-5.rhaos4.5.git1c13d1d.el8
```


```

**Node crc-fd5nx-master-0**

Name:               crc-fd5nx-master-0
Roles:              master,worker
Labels:             beta.kubernetes.io/arch=amd64
                    beta.kubernetes.io/os=linux
                    kubernetes.io/arch=amd64
                    kubernetes.io/hostname=crc-fd5nx-master-0
                    kubernetes.io/os=linux
                    node-role.kubernetes.io/master=
                    node-role.kubernetes.io/worker=
                    node.openshift.io/os_id=rhcos
Annotations:        machine.openshift.io/machine: openshift-machine-api/crc-fd5nx-master-0
                    machineconfiguration.openshift.io/currentConfig: rendered-master-a0c744207a4f0a10c4d584c95bdcf4b9
                    machineconfiguration.openshift.io/desiredConfig: rendered-master-a0c744207a4f0a10c4d584c95bdcf4b9
                    machineconfiguration.openshift.io/reason: 
                    machineconfiguration.openshift.io/state: Done
                    volumes.kubernetes.io/controller-managed-attach-detach: true
CreationTimestamp:  Wed, 29 Jul 2020 04:47:51 +0000
Taints:             <none>
Unschedulable:      false
Lease:
  HolderIdentity:  crc-fd5nx-master-0
  AcquireTime:     <unset>
  RenewTime:       Wed, 13 Oct 2021 01:22:25 +0000
Conditions:
  Type             Status  LastHeartbeatTime                 LastTransitionTime                Reason                       Message
  ----             ------  -----------------                 ------------------                ------                       -------
  MemoryPressure   False   Wed, 13 Oct 2021 01:21:51 +0000   Wed, 29 Jul 2020 04:47:52 +0000   KubeletHasSufficientMemory   kubelet has sufficient memory available
  DiskPressure     False   Wed, 13 Oct 2021 01:21:51 +0000   Wed, 29 Jul 2020 04:47:52 +0000   KubeletHasNoDiskPressure     kubelet has no disk pressure
  PIDPressure      False   Wed, 13 Oct 2021 01:21:51 +0000   Wed, 29 Jul 2020 04:47:52 +0000   KubeletHasSufficientPID      kubelet has sufficient PID available
  Ready            True    Wed, 13 Oct 2021 01:21:51 +0000   Wed, 29 Jul 2020 04:49:33 +0000   KubeletReady                 kubelet is posting ready status
Addresses:
  InternalIP:  192.168.126.11
  Hostname:    crc-fd5nx-master-0
Capacity:
  cpu:                8
  ephemeral-storage:  125275840Ki
  hugepages-1Gi:      0
  hugepages-2Mi:      0
  memory:             22943196Ki
  pods:               250
System Info:
  Machine ID:                              eb3b180bb8a34c7daf567212eb223e8c
  System UUID:                             eb3b180bb8a34c7daf567212eb223e8c
  Boot ID:                                 b16b3a07-d58a-4d2c-a692-830e83f56916
  Kernel Version:                          4.18.0-193.13.2.el8_2.x86_64
  OS Image:                                Red Hat Enterprise Linux CoreOS 45.82.202007240629-0 (Ootpa)
  Operating System:                        linux
  Architecture:                            amd64
  Container Runtime Version:               cri-o://1.18.3-5.rhaos4.5.git1c13d1d.el8
  Kubelet Version:                         v1.18.3+012b3ec
  Kube-Proxy Version:                      v1.18.3+012b3ec
PodCIDR:                                   10.116.0.0/24
PodCIDRs:                                  10.116.0.0/24
Non-terminated Pods:                       (35 in total)
  Namespace                                Name                                                CPU Requests  CPU Limits  Memory Requests  Memory Limits  AGE
  ---------                                ----                                                ------------  ----------  ---------------  -------------  ---
  openshift-apiserver                      apiserver-68f6b5bbf9-r6vhv                          100m (1%)     0 (0%)      200Mi (0%)       0 (0%)         4h9m
  openshift-authentication                 oauth-openshift-855664cd7-2xc97                     10m (0%)      0 (0%)      50Mi (0%)        0 (0%)         4h8m
  openshift-cluster-node-tuning-operator   tuned-rqc66                                         10m (0%)      0 (0%)      50Mi (0%)        0 (0%)         440d
  openshift-config-operator                openshift-config-operator-78bf96dddb-6fxm8          10m (0%)      0 (0%)      50Mi (0%)        0 (0%)         440d
  openshift-console                        console-dc74d4f57-fvwpf                             10m (0%)      0 (0%)      100Mi (0%)       0 (0%)         4h8m
  openshift-console                        downloads-5565cdb86b-ktq2h                          10m (0%)      0 (0%)      50Mi (0%)        0 (0%)         4h8m
  openshift-controller-manager             controller-manager-6slxv                            100m (1%)     0 (0%)      100Mi (0%)       0 (0%)         4h12m
  openshift-dns                            dns-default-22l2z                                   65m (0%)      0 (0%)      110Mi (0%)       512Mi (2%)     440d
  openshift-etcd-operator                  etcd-operator-fcd9d5cb7-qjd9r                       10m (0%)      0 (0%)      50Mi (0%)        0 (0%)         440d
  openshift-etcd                           etcd-crc-fd5nx-master-0                             460m (6%)     0 (0%)      920Mi (4%)       0 (0%)         440d
  openshift-image-registry                 cluster-image-registry-operator-5f47f6fcf7-2n5kk    20m (0%)      0 (0%)      0 (0%)           0 (0%)         440d
  openshift-image-registry                 image-registry-76765c6778-hqb92                     100m (1%)     0 (0%)      256Mi (1%)       0 (0%)         4h10m
  openshift-image-registry                 node-ca-r6wvz                                       10m (0%)      0 (0%)      10Mi (0%)        0 (0%)         440d
  openshift-ingress                        router-default-bc6c7d8fc-pls7j                      100m (1%)     0 (0%)      256Mi (1%)       0 (0%)         4h16m
  openshift-kube-apiserver-operator        kube-apiserver-operator-595f668595-rx8dw            10m (0%)      0 (0%)      50Mi (0%)        0 (0%)         440d
  openshift-kube-apiserver                 kube-apiserver-crc-fd5nx-master-0                   330m (4%)     0 (0%)      1174Mi (5%)      0 (0%)         4h10m
  openshift-kube-controller-manager        kube-controller-manager-crc-fd5nx-master-0          100m (1%)     0 (0%)      500Mi (2%)       0 (0%)         4h12m
  openshift-kube-scheduler                 openshift-kube-scheduler-crc-fd5nx-master-0         20m (0%)      0 (0%)      100Mi (0%)       0 (0%)         4h12m
  openshift-kube-storage-version-migrator  migrator-84d87c7d77-p9m6x                           100m (1%)     0 (0%)      200Mi (0%)       0 (0%)         440d
  openshift-marketplace                    certified-operators-649dc5dc65-rjtnt                10m (0%)      0 (0%)      100Mi (0%)       0 (0%)         4h15m
  openshift-marketplace                    community-operators-544c5b9887-bst7d                10m (0%)      0 (0%)      100Mi (0%)       0 (0%)         440d
  openshift-marketplace                    community-operators-95cc446fb-vwnsl                 10m (0%)      0 (0%)      100Mi (0%)       0 (0%)         4h15m
  openshift-marketplace                    marketplace-operator-df484cccc-dg5vs                10m (0%)      0 (0%)      50Mi (0%)        0 (0%)         440d
  openshift-marketplace                    redhat-marketplace-6b6cbd7d88-g5qwf                 10m (0%)      0 (0%)      100Mi (0%)       0 (0%)         4h15m
  openshift-marketplace                    redhat-operators-8459b87897-9bsl8                   10m (0%) 
     0 (0%)      100Mi (0%)       0 (0%)         4h14m
  openshift-multus                         multus-admission-controller-npr7g                   20m (0%)      0 (0%)      20Mi (0%)        0 (0%)         440d
  openshift-multus                         multus-c6wbs                                        10m (0%)      0 (0%)      150Mi (0%)       0 (0%)         440d
  openshift-operator-lifecycle-manager     catalog-operator-5d4588db56-wtxjv                   10m (0%)      0 (0%)      80Mi (0%)        0 (0%)         440d
  openshift-operator-lifecycle-manager     olm-operator-7d9844479b-nm98h                       10m (0%)      0 (0%)      160Mi (0%)       0 (0%)         440d
  openshift-operator-lifecycle-manager     packageserver-5c49bf9c8d-mqsl7                      0 (0%)        0 (0%)      0 (0%)           0 (0%)         4h10m
  openshift-operator-lifecycle-manager     packageserver-5c49bf9c8d-rdkwq                      0 (0%)        0 (0%)      0 (0%)           0 (0%)         4h14m
  openshift-sdn                            ovs-rsb4q                                           100m (1%)     0 (0%)      400Mi (1%)       0 (0%)         440d
  openshift-sdn                            sdn-controller-bpdpz                                10m (0%)      0 (0%)      50Mi (0%)        0 (0%)         440d
  openshift-sdn                            sdn-k4l75                                           100m (1%)     0 (0%)      200Mi (0%)       0 (0%)         440d
  openshift-service-ca                     service-ca-5dfbf8b8c-xmgr5                          10m (0%)      0 (0%)      120Mi (0%)       0 (0%)         4h13m
Allocated resources:
  (Total limits may be over 100 percent, i.e., overcommitted.)
  Resource           Requests      Limits
  --------           --------      ------
  cpu                1905m (25%)   0 (0%)
  memory             5956Mi (26%)  512Mi (2%)
  ephemeral-storage  0 (0%)        0 (0%)
  hugepages-1Gi      0 (0%)        0 (0%)
  hugepages-2Mi      0 (0%)        0 (0%)
Events:              <none>
```
### Kubernetes config view

```
apiVersion: v1
clusters:
- cluster:
    insecure-skip-tls-verify: true
    server: https://openshift:6443
  name: local
- cluster:
    insecure-skip-tls-verify: true
    server: https://openshift:6443
  name: openshift:6443
contexts:
- context:
    cluster: openshift:6443
    namespace: default
    user: admin
  name: default/openshift:6443/admin
- context:
    cluster: local
    user: ""
  name: local
current-context: default/openshift:6443/admin
kind: Config
preferences: {}
users:
- name: admin
  user:
    token: Gs-v-3czYLTz8OSt81NCeYoSkP_kmKWR4pvv1ZXBTvU
```

### Kubernetes get pods

```
NAMESPACE                                 NAME                                                         READY   STATUS         RESTARTS   AGE     IP               NODE                 NOMINATED NODE   READINESS GATES
openshift-apiserver                       apiserver-68f6b5bbf9-r6vhv                                   1/1     Running        0          4h9m    10.116.0.66      crc-fd5nx-master-0   <none>           <none>
openshift-authentication                  oauth-openshift-855664cd7-2xc97                              1/1     Running        0          4h8m    10.116.0.68      crc-fd5nx-master-0   <none>           <none>
openshift-cluster-node-tuning-operator    tuned-rqc66                                                  1/1     Running        0          440d    192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-config-operator                 openshift-config-operator-78bf96dddb-6fxm8                   1/1     Running        4          440d    10.116.0.16      crc-fd5nx-master-0   <none>           <none>
openshift-console                         console-dc74d4f57-fvwpf                                      1/1     Running        0          4h8m    10.116.0.70      crc-fd5nx-master-0   <none>           <none>
openshift-console                         downloads-5565cdb86b-ktq2h                                   1/1     Running        0          4h8m    10.116.0.71      crc-fd5nx-master-0   <none>           <none>
openshift-controller-manager              controller-manager-6slxv                                     1/1     Running        0          4h12m   10.116.0.46      crc-fd5nx-master-0   <none>           <none>
openshift-dns                             dns-default-22l2z                                            3/3     Running        0          440d    10.116.0.13      crc-fd5nx-master-0   <none>           <none>
openshift-etcd-operator                   etcd-operator-fcd9d5cb7-qjd9r                                1/1     Running        1          440d    10.116.0.32      crc-fd5nx-master-0   <none>           <none>
openshift-etcd                            etcd-crc-fd5nx-master-0                                      4/4     Running        0          440d    192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-etcd                            installer-2-crc-fd5nx-master-0                               0/1     Completed      0          440d    10.116.0.18      crc-fd5nx-master-0   <none>           <none>
openshift-etcd                            revision-pruner-2-crc-fd5nx-master-0                         0/1     Completed      0          440d    10.116.0.38      crc-fd5nx-master-0   <none>           <none>
openshift-image-registry                  cluster-image-registry-operator-5f47f6fcf7-2n5kk             2/2     Running        1          440d    10.116.0.11      crc-fd5nx-master-0   <none>           <none>
openshift-image-registry                  image-pruner-1596067200-dk9x7                                0/1     Completed      0          440d    10.116.0.136     crc-fd5nx-master-0   <none>           <none>
openshift-image-registry                  image-pruner-1634083200-855kv                                0/1     Completed      0          82m     10.116.0.72      crc-fd5nx-master-0   <none>           <none>
openshift-image-registry                  image-registry-76765c6778-hqb92                              1/1     Running        0          4h10m   10.116.0.61      crc-fd5nx-master-0   <none>           <none>
openshift-image-registry                  node-ca-r6wvz                                                1/1     Running        0          440d    192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-ingress                         router-default-bc6c7d8fc-pls7j    
/1     Running        0          4h16m   192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-ingress                         router-default-bc6c7d8fc-wrxnh                               0/1     NodeAffinity   0          440d    <none>           crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver-operator         kube-apiserver-operator-595f668595-rx8dw                     1/1     Running        1          440d    10.116.0.27      crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  installer-10-crc-fd5nx-master-0                              0/1     Completed      0          440d    10.116.0.132     crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  installer-11-crc-fd5nx-master-0                              0/1     Completed      0          4h13m   10.116.0.40      crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  installer-12-crc-fd5nx-master-0                              0/1     Completed      0          4h12m   10.116.0.52      crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  installer-13-crc-fd5nx-master-0                              0/1     Completed      0          4h10m   10.116.0.63      crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  kube-apiserver-crc-fd5nx-master-0                            4/4     Running        0          4h10m   192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  revision-pruner-10-crc-fd5nx-master-0                        0/1     Completed      0          440d    10.116.0.135     crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  revision-pruner-11-crc-fd5nx-master-0                        0/1     Completed      0          4h12m   10.116.0.49      crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  revision-pruner-12-crc-fd5nx-master-0                        0/1     Completed      0          4h11m   10.116.0.54      crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  revision-pruner-13-crc-fd5nx-master-0                        0/1     Completed      0          4h8m    10.116.0.69      crc-fd5nx-master-0   <none>           <none>
openshift-kube-apiserver                  revision-pruner-9-crc-fd5nx-master-0                         0/1     Completed      0          440d    10.116.0.130     crc-fd5nx-master-0   <none>           <none>
openshift-kube-controller-manager         installer-10-crc-fd5nx-master-0                              0/1     Completed      0          4h12m   10.116.0.43      crc-fd5nx-master-0   <none>           <none>
openshift-kube-controller-manager         installer-9-crc-fd5nx-master-0                               0/1     Completed      0          4h13m   10.116.0.39      crc-fd5nx-master-0   <none>           <none>
openshift-kube-controller-manager         kube-controller-manager-crc-fd5nx-master-0                   4/4     Running        2          4h12m   192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-kube-controller-manager         revision-pruner-10-crc-fd5nx-master-0                        0/1     Completed      0          4h12m   10.116.0.53      crc-fd5nx-master-0   <none>           <none>
openshift-kube-controller-manager         revision-pruner-8-crc-fd5nx-master-0                         0/1     Completed      0          440d    10.116.0.134     crc-fd5nx-master-0   <none>           <none>
openshift-kube-controller-manager         revision-pruner-9-crc-fd5nx-master-0                         0/1     Completed      0          4h13m   10.116.0.41      crc-fd5nx-master-0   <none>           <none>
openshift-kube-scheduler                  installer-8-crc-fd5nx-master-0                               0/1     Completed      0          4h12m   10.116.0.42      crc-fd5nx-master-0   <none>           <none>
openshift-kube-scheduler                  openshift-kube-scheduler-crc-fd5nx-master-0                  2/2     Running        1          4h12m   192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-kube-scheduler                  revision-pruner-7-crc-fd5nx-master-0                         0/1     Completed      0          440d    10.116.0.133     crc-fd5nx-master-0   <none>           <none>
openshift-kube-scheduler                  revision-pruner-8-crc-fd5nx-master-0                         0/1     Completed      0          4h11m   10.116.0.55      crc-fd5nx-master-0   <none>           <none>
openshift-kube-storage-version-migrator   migrator-84d87c7d77-p9m6x                                    1/1     Running        0          440d    10.116.0.5       crc-fd5nx-master-0   <none>           <none>
openshift-marketplace                     certified-operators-649dc5dc65-rjtnt                         1/1     Running        1          4h14m   10.116.0.45      crc-fd5nx-master-0   <none>           <none>
openshift-marketplace                     community-operators-544c5b9887-bst7d                         1/1     Running        2          440d    10.116.0.17      crc-fd5nx-master-0   <none>           <none>
openshift-marketplace                     community-operators-95cc446fb-vwnsl                          0/1     Running        56         4h14m   10.116.0.48      crc-fd5nx-master-0   <none>           <none>
openshift-marketplace                     marketplace-operator-df484cccc-dg5vs                         1/1     Running        0          440d    10.116.0.19      crc-fd5nx-master-0   <none>           <none>
openshift-marketplace                     redhat-marketplace-6b6cbd7d88-g5qwf                          1/1     Running        0          4h14m   10.116.0.50      crc-fd5nx-master-0   <none>           <none>
openshift-marketplace                     redhat-operators-8459b87897-9bsl8                            1/1     Running        0          4h14m   10.116.0.51      crc-fd5nx-master-0   <none>           <none>
openshift-multus                          multus-admission-controller-npr7g                            2/2     Running        0          440d    10.116.0.6       crc-fd5nx-master-0   <none>           <none>
openshift-multus                          multus-c6wbs                                                 1/1     Running        0          440d    192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-operator-lifecycle-manager      catalog-operator-5d4588db56-wtxjv                            1/1     Running        0          440d    10.116.0.35      crc-fd5nx-master-0   <none>           <none>
openshift-operator-lifecycle-manager      olm-operator-7d9844479b-nm98h                                1/1     Running        0          440d    10.116.0.38      crc-fd5nx-master-0   <none>           <none>
openshift-operator-lifecycle-manager      packageserver-5c49bf9c8d-mqsl7                               1/1     Running        0          4h10m   10.116.0.57      crc-fd5nx-master-0   <none>           <none>
openshift-operator-lifecycle-manager      packageserver-5c49bf9c8d-rdkwq      
/1     Running        1          4h14m   10.116.0.44      crc-fd5nx-master-0   <none>           <none>
openshift-sdn                             ovs-rsb4q                                                    1/1     Running        0          440d    192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-sdn                             sdn-controller-bpdpz                                         1/1     Running        0          440d    192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-sdn                             sdn-k4l75                                                    1/1     Running        0          440d    192.168.126.11   crc-fd5nx-master-0   <none>           <none>
openshift-service-ca                      service-ca-5dfbf8b8c-xmgr5                                   1/1     Running        0          4h13m   10.116.0.47      crc-fd5nx-master-0   <none>           <none>
openshift-service-catalog-removed         openshift-service-catalog-apiserver-remover-4p5s9            0/1     Completed      0          440d    10.116.0.118     crc-fd5nx-master-0   <none>           <none>
openshift-service-catalog-removed         openshift-service-catalog-controller-manager-remover-mhd6c   0/1     Completed      0          440d    10.116.0.119     crc-fd5nx-master-0   <none>           <none>
```

### Kubernetes get deployment configs

```
```

### Kubernetes Services

```
NAMESPACE                                          NAME                                       TYPE           CLUSTER-IP       EXTERNAL-IP                            PORT(S)                        AGE     SELECTOR
default                                            kubernetes                                 ClusterIP      172.25.0.1       <none>                                 443/TCP                        440d    <none>
default                                            openshift                                  ExternalName   <none>           kubernetes.default.svc.cluster.local   <none>                         440d    <none>
kube-system                                        kubelet                                    ClusterIP      None             <none>                                 10250/TCP,10255/TCP,4194/TCP   440d    <none>
openshift-apiserver-operator                       metrics                                    ClusterIP      172.25.14.58     <none>                                 443/TCP                        440d    app=openshift-apiserver-operator
openshift-apiserver                                api                                        ClusterIP      172.25.69.152    <none>                                 443/TCP                        440d    apiserver=true
openshift-authentication-operator                  metrics                                    ClusterIP      172.25.79.43     <none>                                 443/TCP                        440d    app=authentication-operator
openshift-authentication                           oauth-openshift                            ClusterIP      172.25.29.115    <none>                                 443/TCP                        440d    app=oauth-openshift
openshift-cloud-credential-operator                cco-metrics                                ClusterIP      172.25.196.90    <none>                                 2112/TCP                       440d    app=cloud-credential-operator
openshift-cloud-credential-operator                controller-manager-service                 ClusterIP      172.25.63.16     <none>                                 443/TCP                        440d    control-plane=controller-manager,controller-tools.k8s.io=1.0
openshift-cluster-machine-approver                 machine-approver                           ClusterIP      None             <none>                                 9192/TCP                       440d    app=machine-approver
openshift-cluster-samples-operator                 metrics                                    ClusterIP      None             <none>                                 60000/TCP                      440d    name=cluster-samples-operator
openshift-cluster-storage-operator                 csi-snapshot-controller-operator-metrics   ClusterIP      172.25.28.126    <none>                                 443/TCP                        440d    app=csi-snapshot-controller-operator
openshift-cluster-version                          cluster-version-operator                   ClusterIP      172.25.246.166   <none>                                 9099/TCP                       440d    k8s-app=cluster-version-operator
openshift-config-operator                          metrics                                    ClusterIP      172.25.25.17     <none>                                 443/TCP                        440d    app=openshift-config-operator
openshift-console-operator                         metrics                                    ClusterIP      172.25.128.66    <none>                                 443/TCP                        440d    name
=console-operator
openshift-console                                  console                                    ClusterIP      172.25.237.132   <none>                                 443/TCP                        440d    app=console,component=ui
openshift-console                                  downloads                                  ClusterIP      172.25.183.220   <none>                                 80/TCP                         440d    app=console,component=downloads
openshift-controller-manager-operator              metrics                                    ClusterIP      172.25.127.195   <none>                                 443/TCP                        440d    app=openshift-controller-manager-operator
openshift-controller-manager                       controller-manager                         ClusterIP      172.25.99.8      <none>                                 443/TCP                        440d    controller-manager=true
openshift-dns-operator                             metrics                                    ClusterIP      172.25.117.36    <none>                                 9393/TCP                       440d    name=dns-operator
openshift-dns                                      dns-default                                ClusterIP      172.25.0.10      <none>                                 53/UDP,53/TCP,9154/TCP         440d    dns.operator.openshift.io/daemonset-dns=default
openshift-etcd-operator                            metrics                                    ClusterIP      172.25.139.12    <none>                                 443/TCP                        440d    app=etcd-operator
openshift-etcd                                     etcd                                       ClusterIP      172.25.246.42    <none>                                 2379/TCP,9979/TCP              440d    etcd=true
openshift-etcd                                     host-etcd                                  ClusterIP      None             <none>                                 2379/TCP                       440d    <none>
openshift-etcd                                     host-etcd-2                                ClusterIP      None             <none>                                 2379/TCP                       440d    <none>
openshift-image-registry                           image-registry                             ClusterIP      172.25.199.175   <none>                                 5000/TCP                       440d    docker-registry=default
openshift-image-registry                           image-registry-operator                    ClusterIP 
     None             <none>                                 60000/TCP                      440d    name=cluster-image-registry-operator
openshift-ingress-operator                         metrics                                    ClusterIP      172.25.161.153   <none>                                 9393/TCP                       440d    name=ingress-operator
openshift-ingress                                  router-internal-default                    ClusterIP      172.25.136.223   <none>                                 80/TCP,443/TCP,1936/TCP        440d    ingresscontroller.operator.openshift.io/deployment-ingresscontroller=default
openshift-insights                                 metrics                                    ClusterIP      172.25.92.4      <none>                                 443/TCP                        440d    app=insights-operator
openshift-kube-apiserver-operator                  metrics                                    ClusterIP      172.25.223.176   <none>                                 443/TCP                        440d    app=kube-apiserver-operator
openshift-kube-apiserver                           apiserver                                  ClusterIP      172.25.48.200    <none>                                 443/TCP                        440d    apiserver=true
openshift-kube-controller-manager-operator         metrics                                    ClusterIP      172.25.193.123   <none>                                 443/TCP                        440d    app=kube-controller-manager-operator
openshift-kube-controller-manager                  kube-controller-manager                    ClusterIP      172.25.149.198   <none>                                 443/TCP                        440d    kube-controller-manager=true
openshift-kube-scheduler-operator                  metrics                                    ClusterIP      172.25.140.181   <none>                                 443/TCP                        440d    app=openshift-kube-scheduler-operator
openshift-kube-scheduler                           scheduler                                  ClusterIP      172.25.42.180    <none>                                 443/TCP                        440d    scheduler=true
openshift-kube-storage-version-migrator-operator   metrics                                    ClusterIP      172.25.249.227   <none>                                 443/TCP                        440d    app=kube-storage-version-migrator-operator
openshift-machine-api                              cluster-autoscaler-operator                ClusterIP      172.25.125.62    <none>                                 443/TCP,9192/TCP               440d    k8s-app=cluster-autoscaler-operator
openshift-machine-api                              machine-api-operator                       ClusterIP      172.25.146.79    <none>                                 8443/TCP                       440d    k8s-app=machine-api-operator
openshift-machine-config-operator                  machine-config-daemon                      ClusterIP      172.25.245.131   <none>                                 9001/TCP                       440d    k8s-app=machine-config-daemon
openshift-marketplace                              certified-operators                        ClusterIP      172.25.52.190    <none>                                 50051/TCP                      4h15m   marketplace.operatorSource=certified-operators
openshift-marketplace                              community-operators                        ClusterIP      172.25.32.82     <none>                                 50051/TCP                      4h15m   marketplace.operatorSource=community-operators
openshift-marketplace                              marketplace-operator-metrics               ClusterIP      172.25.103.149   <none>                                 8383/TCP,8081/TCP              440d    name=marketplace-operator
openshift-marketplace                              redhat-marketplace                         ClusterIP      172.25.200.63    <none>                                 50051/TCP                      4h15m   marketplace.operatorSource=redhat-marketplace
openshift-marketplace                              redhat-operators                           ClusterIP      172.25.67.74     <none>                                 50051/TCP                      4h14m   marketplace.operatorSource=redhat-operators
openshift-monitoring                               alertmanager-main                          ClusterIP      172.25.205.236   <none>                                 9094/TCP,9092/TCP              440d    alertmanager=main,app=alertmanager
openshift-monitoring                               alertmanager-operated                      ClusterIP      None             <none>                                 9093/TCP,9094/TCP,9094/UDP     440d    app=alertmanager
openshift-monitoring                               cluster-monitoring-operator                ClusterIP      None             <none>                                 8443/TCP                       440d    app=cluster-monitoring-operator
openshift-monitoring                               grafana                                    ClusterIP      172.25.226.21    <none>                                 3000/TCP                       440d    app=grafana
openshift-monitoring                               kube-state-metrics                         ClusterIP      None             <none>                                 8443/TCP,9443/TCP              440d    app.kubernetes.io/name=kube-state-metrics
openshift-monitoring                               node-exporter                              ClusterIP      None             <none>                                 9100/TCP                       440d    app.kubernetes.io/name=node-exporter,app.kubernetes.io/version=v0.18.1
openshift-monitoring                               openshift-state-metrics                    ClusterIP      None             <none>                                 8443/TCP,9443/TCP              440d    k8s-app=openshift-state-metrics
openshift-monitoring                               prometheus-adapter                         ClusterIP      172.25.163.88    <none>                                 443/TCP                        440d    name=prometheus-adapter
openshift-monitoring                               prometheus-k8s                             ClusterIP      172.25.40.114    <none>                                 9091/TCP,9092/TCP              440d    app=prometheus,prometheus=k8s
openshift-monitoring                               prometheus-operated                        ClusterIP      None             <none>                                 9090/TCP,10901/TCP             440d    app=prometheus
openshift-monitoring                               prometheus-operator                        ClusterIP      None             <none>                                 8443/TCP                       440d    app.kubernetes.io/component=controller,app.kubernetes.io/name=prometheus-operator
openshift-monitoring                               telemeter-client                           ClusterIP      None             <none>                                 8443/TCP                       440d    k8s-app=telemeter-client
openshift-monitoring                               thanos-querier                             ClusterIP      172.25.26.45     <none>                                 9091/TCP,9092/TCP              440d    app.kubernetes.io/component=query-layer,app.kubernetes.io/instance=thanos-querier,app.kubernetes.io/name=thanos-query
openshift-multus                                   multus-admission-controller                ClusterIP      172.25.238.192   <none>                                 443/TCP,8443/TCP               440d    app=multus-admission-controller
openshift-operator-lifecycle-manager               catalog-operator-metrics                   ClusterIP      172.25.173.128   <none>                                 8081/TCP                       440d    app=catalog-operator
openshift-operator-lifecycle-manager               olm-operator-metrics                       ClusterIP      172.25.40.235    <none>                                 8081/TCP                       440d    app=olm-operator
openshift-operator-lifecycle-manager               packageserver-service                      ClusterIP      172.25.188.30    <none>                                 5443/TCP                       4h14m   app=packageserver
openshift-sdn                                      sdn                                        ClusterIP      None             <none>                                 9101/TCP                       440d    app=sdn
openshift-service-ca-operator                      metrics                                    ClusterIP      172.25.211.40    <none>                                 443/TCP                        440d    app=service-ca-operator
```

### Openshift Routes

```
NAMESPACE                  NAME                       HOST/PORT                                                                           PATH   SERVICES            PORT    TERMINATION            WILDCARD
openshift-authentication   katacoda-oauth-openshift   oauth-openshift-2886795275-443-host19nc.environments.katacoda.com                          oauth-openshift     6443    reencrypt/Redirect     None
openshift-authentication   oauth-openshift            oauth-openshift.apps-crc.testing                                                           oauth-openshift     6443    passthrough/Redirect   None
openshift-console          console                    console-openshift-console.apps-crc.testing                                                 console             https   reencrypt/Redirect     None
openshift-console          downloads                  downloads-openshift-console.apps-crc.testing                                               downloads           http    edge/Redirect          None
openshift-console          katacoda-console           console-openshift-console-2886795275-443-host19nc.environments.katacoda.com                console             https   reencrypt/Redirect     None
openshift-image-registry   default-route              default-route-openshift-image-registry.apps-crc.testing                                    image-registry      <all>   reencrypt              None
openshift-monitoring       alertmanager-main          alertmanager-main-openshift-monitoring.apps-crc.testing                                    alertmanager-main   web     reencrypt/Redirect     None
openshift-monitoring       grafana                    grafana-openshift-monitoring.apps-crc.testing                                              grafana             https   reencrypt/Redirect     None
openshift-monitoring       katacoda-grafana           grafana-openshift-monitoring-2886795275-443-host19nc.environments.katacoda.com             grafana             https   reencrypt/Redirect     None
openshift-monitoring       katacoda-prometheus-k8s    prometheus-openshift-monitoring-2886795275-443-host19nc.environments.katacoda.com          prometheus-k8s      web     reencrypt/Redirect     None
openshift-monitoring       prometheus-k8s             prometheus-k8s-openshift-monitoring.apps-crc.testing                                       prometheus-k8s      web     reencrypt/Redirect     None
openshift-monitoring       thanos-querier             thanos-querier-openshift-monitoring.apps-crc.testing                                       thanos-querier      web     reencrypt/Redirect     None
```

### Persistent Volumes

```
NAME     CAPACITY   ACCESS MODES   RECLAIM POLICY   STATUS      CLAIM                                                 STORAGECLASS   REASON   AGE    VOLUMEMODE
pv0001   100Gi      RWO,ROX,RWX    Recycle          Bound       openshift-image-registry/crc-image-registry-storage                           440d   Filesystem
pv0002   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0003   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0004   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0005   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0006   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0007   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0008   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0009   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0010   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0011   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0012   100Gi      RWO,ROX,RWX    Recycle          Available      440d   Filesystem
pv0013   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0014   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0015   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0016   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0017   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0018   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0019   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0020   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0021   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0022   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0023   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0024   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0025   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0026   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0027   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0028   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0029   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
pv0030   100Gi      RWO,ROX,RWX    Recycle          Available                                                                                 440d   Filesystem
```

### Openshift ImageStreams

```
NAMESPACE   NAME                                     IMAGE REPOSITORY                                                                                           TAGS                                                  UPDATED
openshift   apicast-gateway                          default-route-openshift-image-registry.apps-crc.testing/openshift/apicast-gateway                          2.1.0.GA,2.2.0.GA,2.3.0.GA,2.4.0.GA + 5 more...       14 months ago
openshift   apicurito-ui                             default-route-openshift-image-registry.apps-crc.testing/openshift/apicurito-ui                             1.2,1.3,1.4,1.5                                       14 months ago
openshift   cli                                      default-route-openshift-image-registry.apps-crc.testing/openshift/cli                                      latest                                                14 months ago
openshift   cli-artifacts                            default-route-openshift-image-registry.apps-crc.testing/openshift/cli-artifacts                            latest                                                14 months ago
openshift   dotnet                                   default-route-openshift-image-registry.apps-crc.testing/openshift/dotnet                                   2.1,3.1,latest                                        14 months ago
openshift   dotnet-runtime                           default-route-openshift-image-registry.apps-crc.testing/openshift/dotnet-runtime                           2.1,3.1,latest                                        14 months ago
openshift   eap-cd-openshift                         default-route-openshift-image-registry.apps-crc.testing/openshift/eap-cd-openshift                         12,12.0,13,13.0,14,14.0,15,15.0,16,16.0 + 5 more...   14 months ago
openshift   eap-cd-runtime-openshift                 default-route-openshift-image-registry.apps-crc.testing/openshift/eap-cd-runtime-openshift                 18,18.0,latest                                        14 months ago
openshift   fis-java-openshift                       default-route-openshift-image-registry.apps-crc.testing/openshift/fis-java-openshift                       1.0,2.0                                               14 months ago
openshift   fis-karaf-openshift                      default-route-openshift-image-registry.apps-crc.testing/openshift/fis-karaf-openshift                      1.0,2.0                                               14 months ago
openshift   fuse-apicurito-generator                 default-route-openshift-image-registry.apps-crc.testing/openshift/fuse-apicurito-generator                 1.2,1.3,1.4,1.5                                       14 months ago
openshift   fuse7-console                            default-route-openshift-image-registry.apps-crc.testing/openshift/fuse7-console                            1.0,1.1,1.2,1.3,1.4,1.5                               14 months ago
openshift   fuse7-eap-openshift                      default-route-openshift-image-registry.apps-crc.testing/openshift/fuse7-eap-openshift                      1.0,1.1,1.2,1.3,1.4,1.5                               14 months ago
openshift   fuse7-java-openshift                     default-route-openshift-image-registry.apps-crc.testing/openshift/fuse7-java-openshift                     1.0,1.1,1.2,1.3,1.4,1.5                               14 months ago
openshift   fuse7-karaf-openshift                    default-route-openshift-image-registry.apps-crc.testing/openshift/fuse7-karaf-openshift                    1.0,1.1,1.2,1.3,1.4,1.5                               14 months ago
openshift   golang                                   default-route-openshift-image-registry.apps-crc.testing/openshift/golang                                   1.11.5,latest                                         14 months ago
openshift   httpd                                    default-route-openshift-image-registry.apps-crc.testing/openshift/httpd                                    2.4,latest                                            14 months ago
openshift   installer                                default-route-openshift-image-registry.apps-crc.testing/openshift/installer                                latest                                                14 months ago
openshift   installer-artifacts                      default-route-openshift-image-registry.apps-crc.testing/openshift/installer-artifacts                      latest                                                14 months ago
openshift   java                                     default-route-openshift-image-registry.apps-crc.testing/openshift/java                                     11,8,latest                                           14 months ago
openshift   jboss-amq-62                             default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-amq-62                             1.1,1.2,1.3,1.4,1.5,1.6,1.7                           14 months ago
openshift   jboss-amq-63                             default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-amq-63                             1.0,1.1,1.2,1.3,1.4                                   14 months ago
openshift   jboss-datagrid65-client-openshift        default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-datagrid65-client-openshift        1.0,1.1                                               14 months ago
openshift   jboss-datagrid65-openshift               default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-datagrid65-openshift               1.2,1.3,1.4,1.5,1.6                                   14 months ago
openshift   jboss-datagrid71-client-openshift        default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-datagrid71-client-openshift        1.0                                                   14 months ago
openshift   jboss-datagrid71-openshift               default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-datagrid71-openshift               1.0,1.1,1.2,1.3                                       14 months ago
openshift   jboss-datagrid72-openshift               default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-datagrid72-openshift               1.0,1.1,1.2                                           14 months ago
openshift   jboss-datagrid73-openshift               default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-datagrid73-openshift               1.0,1.1,1.2,1.3,1.4                                   14 months ago
openshift   jboss-datavirt64-driver-openshift        default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-datavirt64-driver-openshift        1.0,1.1,1.2,1.3,1.4,1.5,1.6,1.7                       14 months ago
openshift   jboss-datavirt64-openshift               default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-datavirt64-openshift               1.0,1.1,1.2,1.3,1.4,1.5,1.6,1.7                       14 months ago
openshift   jboss-decisionserver64-openshift         default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-decisionserver64-openshift         1.0,1.1,1.2,1.3,1.4,1.5,1.6                           14 months ago
openshift   jboss-eap64-openshift                    default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-eap64-openshift                    1.1,1.2,1.3,1.4,1.5,1.6,1.7,1.8,1.9 + 1 more...       14 months ago
openshift   jboss-eap70-openshift                    default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-eap70-openshift                    1.3,1.4,1.5,1.6,1.7                                   14 months ago
openshift   jboss-eap71-openshift                    default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-eap71-openshift                    1.1,1.2,1.3,1.4,latest                                14 months ago
openshift   jboss-eap72-openshift                    default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-eap72-openshift                    1.0,1.1,1.2,latest                                    14 months ago
openshift   jboss-fuse70-console                     default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-fuse70-console                     1.0                                                   14 months ago
openshift   jboss-fuse70-eap-openshift               default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-fuse70-eap-openshift               1.0                                                   14 months ago
openshift   jboss-fuse70-java-openshift              default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-fuse70-java-openshift              1.0                                                   14 months ago
openshift   jboss-fuse70-karaf-openshift             default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-fuse70-karaf-openshift             1.0                                                   14 months ago
openshift   jboss-processserver64-openshift          default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-processserver64-openshift          1.0,1.1,1.2,1.3,1.4,1.5,1.6                           14 months ago
openshift   jboss-webserver30-tomcat7-openshift      default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-webserver30-tomcat7-openshift      1.1,1.2,1.3                                           14 months ago
openshift   jboss-webserver30-tomcat8-openshift      default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-webserver30-tomcat8-openshift      1.1,1.2,1.3                                           14 months ago
openshift   jboss-webserver31-tomcat7-openshift      default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-webserver31-tomcat7-openshift      1.0,1.1,1.2,1.3,1.4                                   14 months ago
openshift   jboss-webserver31-tomcat8-openshift      default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-webserver31-tomcat8-openshift      1.0,1.1,1.2,1.3,1.4                                   14 months ago
openshift   jboss-webserver50-tomcat9-openshift      default-route-openshift-image-registry.apps-crc.testing/openshift/jboss-webserver50-tomcat9-openshift      1.0,1.1,1.2,latest                                    14 months ago
openshift   jenkins                                  default-route-openshift-image-registry.apps-crc.testing/openshift/jenkins                                  2,latest                                              14 months ago
openshift   jenkins-agent-maven                      default-route-openshift-image-registry.apps-crc.testing/openshift/jenkins-agent-maven                      latest,v4.0                                           14 months ago
openshift   jenkins-agent-nodejs                     default-route-openshift-image-registry.apps-crc.testing/openshift/jenkins-agent-nodejs                     latest,v4.0                                           14 months ago
openshift   mariadb                                  default-route-openshift-image-registry.apps-crc.testing/openshift/mariadb                                  10.2,10.3,latest                                      14 months ago
openshift   mongodb                                  default-route-openshift-image-registry.apps-crc.testing/openshift/mongodb                                  3.4,3.6,latest                                        14 months ago
openshift   must-gather                              default-route-openshift-image-registry.apps-crc.testing/openshift/must-gather                              latest                                                14 months ago
openshift   mysql                                    default-route-openshift-image-registry.apps-crc.testing/openshift/mysql                                    5.7,8.0,latest                                        14 months ago
openshift   nginx                                    default-route-openshift-image-registry.apps-crc.testing/openshift/nginx                                    1.10,1.14,1.16,latest                                 14 months ago
openshift   nodejs                                   default-route-openshift-image-registry.apps-crc.testing/openshift/nodejs                                   10,12,latest                                          14 months ago
openshift   oauth-proxy                              default-route-openshift-image-registry.apps-crc.testing/openshift/oauth-proxy                              v4.4                                                  14 months ago
openshift   openjdk-11-rhel7                         default-route-openshift-image-registry.apps-crc.testing/openshift/openjdk-11-rhel7                         1.0,1.1                                               14 months ago
openshift   openjdk-11-rhel8                         default-route-openshift-image-registry.apps-crc.testing/openshift/openjdk-11-rhel8                         1.0                                                   14 months ago
openshift   openjdk-8-rhel8                          default-route-openshift-image-registry.apps-crc.testing/openshift/openjdk-8-rhel8                          1.0,1.1,1.2                                           14 months ago
openshift   perl                                     default-route-openshift-image-registry.apps-crc.testing/openshift/perl                                     5.26,latest                                           14 months ago
openshift   php                                      default-route-openshift-image-registry.apps-crc.testing/openshift/php                                      7.2,7.3,latest                                        14 months ago
openshift   postgresql                               default-route-openshift-image-registry.apps-crc.testing/openshift/postgresql                               10,12,9.6,latest                                      14 months ago
openshift   python                                   default-route-openshift-image-registry.apps-crc.testing/openshift/python                                   2.7,3.6,latest                                        14 months ago
openshift   redhat-openjdk18-openshift               default-route-openshift-image-registry.apps-crc.testing/openshift/redhat-openjdk18-openshift               1.0,1.1,1.2,1.3,1.4,1.5,1.6,1.7,1.8                   14 months ago
openshift   redhat-sso70-openshift                   default-route-openshift-image-registry.apps-crc.testing/openshift/redhat-sso70-openshift                   1.3,1.4                                               14 months ago
openshift   redhat-sso71-openshift                   default-route-openshift-image-registry.apps-crc.testing/openshift/redhat-sso71-openshift                   1.0,1.1,1.2,1.3                                       14 months ago
openshift   redhat-sso72-openshift                   default-route-openshift-image-registry.apps-crc.testing/openshift/redhat-sso72-openshift                   1.0,1.1,1.2,1.3,1.4                                   14 months ago
openshift   redhat-sso73-openshift                   default-route-openshift-image-registry.apps-crc.testing/openshift/redhat-sso73-openshift                   1.0,latest										      14 months ago
openshift   redis                                    default-route-openshift-image-registry.apps-crc.testing/openshift/redis                                    5,latest                                              14 months ago
openshift   rhdm-decisioncentral-rhel8               default-route-openshift-image-registry.apps-crc.testing/openshift/rhdm-decisioncentral-rhel8               7.7.0                                                 14 months ago
openshift   rhdm-kieserver-rhel8                     default-route-openshift-image-registry.apps-crc.testing/openshift/rhdm-kieserver-rhel8                     7.7.0                                                 14 months ago
openshift   rhpam-businesscentral-monitoring-rhel8   default-route-openshift-image-registry.apps-crc.testing/openshift/rhpam-businesscentral-monitoring-rhel8   7.7.0                                                 14 months ago
openshift   rhpam-businesscentral-rhel8              default-route-openshift-image-registry.apps-crc.testing/openshift/rhpam-businesscentral-rhel8              7.7.0                                                 14 months ago
openshift   rhpam-kieserver-rhel8                    default-route-openshift-image-registry.apps-crc.testing/openshift/rhpam-kieserver-rhel8                    7.7.0                                                 14 months ago
openshift   rhpam-smartrouter-rhel8                  default-route-openshift-image-registry.apps-crc.testing/openshift/rhpam-smartrouter-rhel8                  7.7.0                                                 14 months ago
openshift   ruby                                     default-route-openshift-image-registry.apps-crc.testing/openshift/ruby                                     2.4,2.5,2.6,latest                                    14 months ago
openshift   sso74-openshift-rhel8                    default-route-openshift-image-registry.apps-crc.testing/openshift/sso74-openshift-rhel8                    7.4,latest                                            14 months ago
openshift   tests                                    default-route-openshift-image-registry.apps-crc.testing/openshift/tests                                    latest                                                14 months ago
openshift   tools                                    default-route-openshift-image-registry.apps-crc.testing/openshift/tools                                    latest                                                14 months ago
```
### Openshift Build Templates (S2I)

```
Templates (oc new-app --template=<template>)
-----
sso74-postgresql
  Project: openshift
  An example application based on RH-SSO 7.4 on OpenJDK image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/tree/sso74-dev/docs.
sso74-ocp4-x509-postgresql-persistent
  Project: openshift
  An example application based on RH-SSO 7.4 on OpenJDK image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/tree/sso74-dev/docs.
sso74-ocp4-x509-https
  Project: openshift
  An example application based on RH-SSO 7.4 on OpenJDK image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/tree/sso74-dev/docs.
sso74-https
  Project: openshift
  An example application based on RH-SSO 7.4 on OpenJDK image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/tree/sso74-dev/docs.
sso73-postgresql-persistent
  Project: openshift
  An example application based on RH-SSO 7.3 image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/docs.
sso73-postgresql
  Project: openshift
  An example application based on RH-SSO 7.3 image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/docs.
sso73-ocp4-x509-postgresql-persistent
  Project: openshift
  An example application based on RH-SSO 7.3 image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/docs.
3scale-gateway
  Project: openshift
  3scale's APIcast is an NGINX based API gateway used to integrate your internal and external API services with 3scale's API Management Platform. It supports OpenID connect to integrate with external Identity Providers such as Red Hat Single Sign On, for API traffic authentication
amq63-basic
  Project: openshift
  Application template for JBoss A-MQ brokers. These can be deployed as standalone or in a mesh. This template doesn't feature SSL support.
amq63-persistent
  Project: openshift
  An example JBoss A-MQ application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
amq63-persistent-ssl
  Project: openshift
  An example JBoss A-MQ application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
amq63-ssl
  Project: openshift
  An example JBoss A-MQ application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
apicurito
  Project: openshift
  Design beautiful, functional APIs with zero coding, using a visual designer for OpenAPI documents.
cache-service
  Project: openshift
  Red Hat Data Grid is an in-memory, distributed key/value store.
cakephp-mysql-example
  Project: openshift
  An example CakePHP application with a MySQL database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/cakephp-ex/blob/master/README.md.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing.
cakephp-mysql-persistent
  Project: openshift
  An example CakePHP application with a MySQL database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/cakephp-ex/blob/master/README.md.
dancer-mysql-example
  Project: openshift
  An example Dancer application with a MySQL database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/dancer-ex/blob/master/README.md.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing.
dancer-mysql-persistent
  Project: openshift
  An example Dancer application with a MySQL database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/dancer-ex/blob/master/README.md.
datagrid-service
  Project: openshift
  Red Hat Data Grid is an in-memory, distributed key/value store.
datavirt64-basic-s2i
  Project: openshift
  Application template for JBoss Data Virtualization 6.4 services built using S2I.
datavirt64-extensions-support-s2i
  Project: openshift
  An example JBoss Data Virtualization application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
datavirt64-ldap-s2i
  Project: openshift
  Application template for JBoss Data Virtualization 6.4 services that configures security domain using S2I.
datavirt64-secure-s2i
  Project: openshift
  An example JBoss Data Virtualization application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
decisionserver64-amq-s2i
  Project: openshift
  An example BRMS decision server A-MQ application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
decisionserver64-basic-s2i
  Project: openshift
  Application template for Red Hat JBoss BRMS 6.4 decision server applications built using S2I.
django-psql-example
  Project: openshift
  An example Django application with a PostgreSQL database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/django-ex/blob/master/README.md.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing.
django-psql-persistent
  Project: openshift
  An example Django application with a PostgreSQL database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/django-ex/blob/master/README.md.
dotnet-example
  Project: openshift
  An example .NET Core application.
dotnet-pgsql-persistent
  Project: openshift
  An example .NET Core application with a PostgreSQL database. For more information about using this template, including OpenShift considerations, see https://github.com/redhat-developer/s2i-dotnetcore.
eap-cd-basic-s2i
  Project: openshift
  An example JBoss Enterprise Application Platform continuous delivery application. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap-cd/README.adoc
eap-cd-starter-s2i
  Project: openshift
  An example JBoss Enterprise Application Platform continuous delivery application. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap-cd/README.adoc
eap72-basic-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc
eap72-https-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application configured with secure communication using HTTPS. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc
eap72-mongodb-persistent-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application with a MongoDB database. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc.
eap72-mongodb-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application with a MongoDB database. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc.
eap72-mysql-persistent-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7.2 application with a persistent MySQL database. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc.
eap72-mysql-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application with a MySQL database. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc.
eap72-postgresql-persistent-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application with a persistent PostgreSQL database. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc
eap72-postgresql-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application with an PostgreSQL database configured with secure communication using https and ephemeral storage. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc
eap72-sso-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application Single Sign-On application. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc
eap72-third-party-db-s2i
  Project: openshift
  An example Red Hat JBoss EAP 7 application. For more information about using this template, see https://github.com/jboss-container-images/jboss-eap-7-openshift-image/blob/eap72/README.adoc.
fuse75-console
  Project: openshift
  The Red Hat Fuse Console eases the discovery and management of Fuse applications deployed on OpenShift.
fuse76-console
  Project: openshift
  The Red Hat Fuse Console eases the discovery and management of Fuse applications deployed on OpenShift.
httpd-example
  Project: openshift
  An example Apache HTTP Server (httpd) application that serves static content. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/httpd-ex/blob/master/README.md.
jenkins-ephemeral
  Project: openshift
  Jenkins service, without persistent storage.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing.
jenkins-ephemeral-monitored
  Project: openshift
  Jenkins service, without persistent storage.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing.
jenkins-persistent
  Project: openshift
  Jenkins service, with persistent storage.

NOTE: You must have persistent volumes available in your cluster to use this template.
jenkins-persistent-monitored
  Project: openshift
  Jenkins service, with persistent storage.

NOTE: You must have persistent volumes available in your cluster to use this template.
jws31-tomcat7-basic-s2i
  Project: openshift
  Application template for JWS applications built using S2I.
jws31-tomcat7-https-s2i
  Project: openshift
  An example JBoss Web Server application configured for use with https. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws31-tomcat7-mongodb-persistent-s2i
  Project: openshift
  An example JBoss Web Server application with a MongoDB database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws31-tomcat7-mongodb-s2i
  Project: openshift
  Application template for JWS MongoDB applications built using S2I.
jws31-tomcat7-mysql-persistent-s2i
  Project: openshift
  An example JBoss Web Server application with a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws31-tomcat7-mysql-s2i
  Project: openshift
  Application template for JWS MySQL applications built using S2I.
sso73-ocp4-x509-https
  Project: openshift
  An example application based on RH-SSO 7.3 image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/docs.
jws31-tomcat7-postgresql-s2i
  Project: openshift
  Application template for JWS PostgreSQL applications built using S2I.
jws31-tomcat8-basic-s2i
  Project: openshift
  An example JBoss Web Server application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws31-tomcat8-https-s2i
  Project: openshift
  An example JBoss Web Server application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws31-tomcat8-mongodb-persistent-s2i
  Project: openshift
  An example JBoss Web Server application with a MongoDB database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws31-tomcat8-mongodb-s2i
  Project: openshift
  Application template for JWS MongoDB applications built using S2I.
jws31-tomcat8-mysql-persistent-s2i
  Project: openshift
  An example JBoss Web Server application with a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws31-tomcat8-mysql-s2i
  Project: openshift
  Application template for JWS MySQL applications built using S2I.
jws31-tomcat8-postgresql-persistent-s2i
  Project: openshift
  Application template for JWS PostgreSQL applications with persistent storage built using S2I.
jws50-tomcat9-basic-s2i
  Project: openshift
  An example JBoss Web Server application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws50-tomcat9-https-s2i
  Project: openshift
  An example JBoss Web Server application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws50-tomcat9-mongodb-persistent-s2i
  Project: openshift
  An example JBoss Web Server application with a MongoDB database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws50-tomcat9-mongodb-s2i
  Project: openshift
  Application template for JWS MongoDB applications built using S2I.
jws50-tomcat9-mysql-persistent-s2i
  Project: openshift
  An example JBoss Web Server application with a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
jws50-tomcat9-mysql-s2i
  Project: openshift
  Application template for JWS MySQL applications built using S2I.
jws50-tomcat9-postgresql-persistent-s2i
  Project: openshift
  Application template for JWS PostgreSQL applications with persistent storage built using S2I.
mariadb-ephemeral
  Project: openshift
  MariaDB database service, without persistent storage. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/mariadb-container/blob/master/10.2/root/usr/share/container-scripts/mysql/README.md.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing
mariadb-persistent
  Project: openshift
  MariaDB database service, with persistent storage. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/mariadb-container/blob/master/10.2/root/usr/share/container-scripts/mysql/README.md.

NOTE: Scaling to more than one replica is not supported. You must have persistent volumes available in your cluster to use this template.
mongodb-ephemeral
  Project: openshift
  MongoDB database service, without persistent storage. For more information about using this template, including OpenShift considerations, see documentation in the upstream repository: https://github.com/sclorg/mongodb-container.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing
mongodb-persistent
  Project: openshift
  MongoDB database service, with persistent storage. For more information about using this template, including OpenShift considerations, see documentation in the upstream repository: https://github.com/sclorg/mongodb-container.

NOTE: Scaling to more than one replica is not supported. You must have persistent volumes available in your cluster to use this template.
mysql-ephemeral
  Project: openshift
  MySQL database service, without persistent storage. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/mysql-container/blob/master/8.0/root/usr/share/container-scripts/mysql/README.md.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing
mysql-persistent
  Project: openshift
  MySQL database service, with persistent storage. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/mysql-container/blob/master/8.0/root/usr/share/container-scripts/mysql/README.md.

NOTE: Scaling to more than one replica is not supported. You must have persistent volumes available in your cluster to use this template.
nginx-example
  Project: openshift
  An example Nginx HTTP server and a reverse proxy (nginx) application that serves static content. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/nginx-ex/blob/master/README.md.
nodejs-mongo-persistent
  Project: openshift
  An example Node.js application with a MongoDB database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/nodejs-ex/blob/master/README.md.
nodejs-mongodb-example
  Project: openshift
  An example Node.js application with a MongoDB database. For more information about using this template
, including OpenShift considerations, see https://github.com/sclorg/nodejs-ex/blob/master/README.md.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing.
openjdk-web-basic-s2i
  Project: openshift
  An example Java application using OpenJDK. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
postgresql-ephemeral
  Project: openshift
  PostgreSQL database service, without persistent storage. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/postgresql-container/.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing
postgresql-persistent
  Project: openshift
  PostgreSQL database service, with persistent storage. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/postgresql-container/.

NOTE: Scaling to more than one replica is not supported. You must have persistent volumes available in your cluster to use this template.
processserver64-amq-mysql-persistent-s2i
  Project: openshift
  An example BPM Suite application with A-MQ and a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
processserver64-amq-mysql-s2i
  Project: openshift
  An example BPM Suite application with A-MQ and a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
processserver64-amq-postgresql-persistent-s2i
  Project: openshift
  An example BPM Suite application with A-MQ and a PostgreSQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
processserver64-amq-postgresql-s2i
  Project: openshift
  An example BPM Suite application with A-MQ and a PostgreSQL database. For more information about using
 this template, see https://github.com/jboss-openshift/application-templates.
processserver64-basic-s2i
  Project: openshift
  An example BPM Suite application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
processserver64-externaldb-s2i
  Project: openshift
  An example BPM Suite application with a external database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
processserver64-mysql-persistent-s2i
  Project: openshift
  An example BPM Suite application with a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
processserver64-mysql-s2i
  Project: openshift
  An example BPM Suite application with a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
processserver64-postgresql-persistent-s2i
  Project: openshift
  An example BPM Suite application with a PostgreSQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
rails-pgsql-persistent
  Project: openshift
  An example Rails application with a PostgreSQL database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/rails-ex/blob/master/README.md.
rails-postgresql-example
  Project: openshift
  An example Rails application with a PostgreSQL database. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/rails-ex/blob/master/README.md.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing.
redis-ephemeral
  Project: openshift
  Redis in-memory data structure store, without persistent storage. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/redis-container/blob/master/5.

WARNING: Any data stored will be lost upon pod destruction. Only use this template for testing
redis-persistent
  Project: openshift
  Redis in-memory data structure store, with persistent storage. For more information about using this template, including OpenShift considerations, see https://github.com/sclorg/redis-container/blob/master/5.

NOTE: You must have persistent volumes available in your cluster to use this template.
rhdm77-authoring
  Project: openshift
  Application template for a non-HA persistent authoring environment, for Red Hat Decision Manager 7.7 - Deprecated
rhdm77-authoring-ha
  Project: openshift
  Application template for a HA persistent authoring environment, for Red Hat Decision Manager 7.7 - Deprecated
rhdm77-kieserver
  Project: openshift
  Application template for a managed KIE Server, for Red Hat Decision Manager 7.7 - Deprecated
rhdm77-prod-immutable-kieserver
  Project: openshift
  Application template for an immutable KIE server in a production environment, for Red Hat Decision Manager 7.7 - Deprecated
rhdm77-prod-immutable-kieserver-amq
  Project: openshift
  Application template for an immutable KIE server in a production environment integrated with ActiveMQ, for Red Hat Decision Manager 7.7 - Deprecated
rhdm77-trial-ephemeral
  Project: openshift
  Application template for an ephemeral authoring and testing environment, for Red Hat Decision Manager 7.7 - Deprecated
rhpam77-authoring
  Project: openshift
  Application template for a non-HA persistent authoring environment, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-authoring-ha
  Project: openshift
  Application template for a HA persistent authoring environment, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-kieserver-externaldb
  Project: openshift
  Application template for a managed KIE Server with an external database, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-kieserver-mysql
  Project: openshift
  Application template for a managed KIE Server with a MySQL database, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-kieserver-postgresql
  Project: openshift
  Application template for a managed KIE Server with a PostgreSQL database, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-managed
  Project: openshift
  Application template for a managed HA production runtime environment, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-prod
  Project: openshift
  Application template for a managed HA production runtime environment, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-prod-immutable-kieserver
  Project: openshift
  Application template for an immutable KIE server in a production environment, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-prod-immutable-kieserver-amq
  Project: openshift
  Application template for an immutable KIE server in a production environment integrated with ActiveMQ, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-prod-immutable-monitor
  Project: openshift
  Application template for a router and monitoring console in a production environment, for Red Hat Process Automation Manager 7.7 - Deprecated
rhpam77-trial-ephemeral
  Project: openshift
  Application template for an ephemeral authoring and testing environment, for Red Hat Process Automation Manager 7.7 - Deprecated
s2i-fuse75-spring-boot-camel
  Project: openshift
  Spring Boot and Camel QuickStart. This example demonstrates how you can use Apache Camel with Spring Boot on OpenShift. The quickstart uses Spring Boot to configure an application which includes a Camel route that triggers a message every 5th second, and routes the message to a log.
s2i-fuse75-spring-boot-camel-rest-3scale
  Project: openshift
  Spring Boot, Camel REST DSL and 3Scale QuickStart. This example demonstrates how to use Camel's REST DSL to expose a RESTful API and expose it to 3scale.
s2i-fuse75-spring-boot-camel-xml
  Project: openshift
  Spring Boot and Camel Xml QuickStart. This example demonstrates how you can use Apache Camel with Spring Boot on OpenShift. The quickstart uses Spring Boot to configure an application which includes a Camel route (in Spring xml) that triggers a message every 5th second, and routes the message to a log.
s2i-fuse76-spring-boot-camel
  Project: openshift
  Spring Boot and Camel QuickStart. This example demonstrates how you can use Apache Camel with Spring Boot on OpenShift. The quickstart uses Spring Boot to configure an application which includes a Camel route that triggers a message every 5th second, and routes the message to a log.
s2i-fuse76-spring-boot-camel-rest-3scale
  Project: openshift
  Spring Boot, Camel REST DSL and 3Scale QuickStart. This example demonstrates how to use Camel's REST DSL to expose a RESTful API and expose it to 3scale.
s2i-fuse76-spring-boot-camel-xml
  Project: openshift
  Spring Boot and Camel Xml QuickStart. This example demonstrates how you can use Apache Camel with Spring Boot on OpenShift. The quickstart uses Spring Boot to configure an application which includes a Camel route (in Spring xml) that triggers a message every 5th second, and routes the message to a log.
sso72-https
  Project: openshift
  An example RH-SSO 7 application. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
sso72-mysql
  Project: openshift
  An example RH-SSO 7 application with a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
sso72-mysql-persistent
  Project: openshift
  An example RH-SSO 7 application with a MySQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
sso72-postgresql
  Project: openshift
  An example RH-SSO 7 application with a PostgreSQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
sso72-postgresql-persistent
  Project: openshift
  An example RH-SSO 7 application with a PostgreSQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
sso73-https
  Project: openshift
  An example application based on RH-SSO 7.3 image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/docs.
sso73-mysql
  Project: openshift
  An example application based on RH-SSO 7.3 image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/docs.
sso73-mysql-persistent
  Project: openshift
  An example application based on RH-SSO 7.3 image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/docs.
jws31-tomcat7-postgresql-persistent-s2i
  Project: openshift
  An example JBoss Web Server application with a PostgreSQL database. For more information about using this template, see https://github.com/jboss-openshift/application-templates.
sso73-ocp4-x509-mysql-persistent
  Project: openshift
  An example application based on RH-SSO 7.3 image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/docs.
sso74-postgresql-persistent
  Project: openshift
  An example application based on RH-SSO 7.4 on OpenJDK image. For more information about using this template, see https://github.com/jboss-container-images/redhat-sso-7-openshift-image/tree/sso74-dev/docs.

Image streams (oc new-app --image-stream=<image-stream> [--code=<source>])
-----
apicast-gateway
  Project: openshift
  Tags:    2.1.0.GA, 2.2.0.GA, 2.3.0.GA, 2.4.0.GA, 2.5.0.GA, 2.6.0.GA, 2.7.0.GA, 2.8.0.GA, latest
cli
  Project: openshift
  Tags:    latest
cli-artifacts
  Project: openshift
  Tags:    latest
dotnet
  Project: openshift
  Tags:    2.1, 3.1, latest
dotnet-runtime
  Project: openshift
  Tags:    2.1, 3.1, latest
golang
  Project: openshift
  Tags:    1.11.5, latest
httpd
  Project: openshift
  Tags:    2.4, latest
installer
  Project: openshift
  Tags:    latest
installer-artifacts
  Project: openshift
  Tags:    latest
java
  Project: openshift
  Tags:    11, 8, latest
jenkins
  Project: openshift
  Tags:    2, latest
jenkins-agent-maven
  Project: openshift
  Tags:    latest, v4.0
jenkins-agent-nodejs
  Project: openshift
  Tags:    latest, v4.0
mariadb
  Project: openshift
  Tags:    10.2, 10.3, latest
mongodb
  Project: openshift
  Tags:    3.4, 3.6, latest
must-gather
  Project: openshift
  Tags:    latest
mysql
  Project: openshift
  Tags:    5.7, 8.0, latest
tests
  Project: openshift
  Tags:    latest
nodejs
  Project: openshift
  Tags:    10, 12, latest
perl
  Project: openshift
  Tags:    5.26, latest
php
  Project: openshift
  Tags:    7.2, 7.3, latest
postgresql
  Project: openshift
  Tags:    10, 12, 9.6, latest
python
  Project: openshift
  Tags:    2.7, 3.6, latest
redis
  Project: openshift
  Tags:    5, latest
ruby
  Project: openshift
  Tags:    2.4, 2.5, 2.6, latest
sso74-openshift-rhel8
  Project: openshift
  Tags:    latest
  Red Hat Single Sign-On 7.4 on OpenJDK
nginx
  Project: openshift
  Tags:    1.10, 1.14, 1.16, latest
tools
  Project: openshift
  Tags:    latest
rhpam-kieserver-rhel8
  Project: openshift
  Tags:    7.7.0
rhpam-businesscentral-rhel8
  Project: openshift
  Tags:    7.7.0
rhpam-businesscentral-monitoring-rhel8
  Project: openshift
  Tags:    7.7.0
rhdm-kieserver-rhel8
  Project: openshift
  Tags:    7.7.0
rhdm-decisioncentral-rhel8
  Project: openshift
  Tags:    7.7.0
oauth-proxy
  Project: openshift
  Tags:    v4.4
rhpam-smartrouter-rhel8
  Project: openshift
  Tags:    7.7.0

```

### Openshift BuildConfigs

```
```

### Failed Pods per NS


*Failed pods in namespace: default*

```
```

*Failed pods in namespace: kube-node-lease*

```
```

*Failed pods in namespace: kube-public*
```
```

*Failed pods in namespace: kube-system*

```
```

*Failed pods in namespace: openshift*

```
```

*Failed pods in namespace: openshift-apiserver*

```
```

*Failed pods in namespace: openshift-apiserver-operator*

```
```

*Failed pods in namespace: openshift-authentication*

```
```

*Failed pods in namespace: openshift-authentication-operator*

```
```

*Failed pods in namespace: openshift-cloud-credential-operator*
```
```

*Failed pods in namespace: openshift-cluster-machine-approver*

```
```

*Failed pods in namespace: openshift-cluster-node-tuning-operator*

```
```

*Failed pods in namespace: openshift-cluster-samples-operator*

```
```

*Failed pods in namespace: openshift-cluster-storage-operator*

```
```

*Failed pods in namespace: openshift-cluster-version*

```
```

*Failed pods in namespace: openshift-config*

```
```

*Failed pods in namespace: openshift-config-managed*
```
```

*Failed pods in namespace: openshift-config-operator*

```
```

*Failed pods in namespace: openshift-console*

```
```

*Failed pods in namespace: openshift-console-operator*

```
```

*Failed pods in namespace: openshift-controller-manager*

```
```

*Failed pods in namespace: openshift-controller-manager-operator*

```
```

*Failed pods in namespace: openshift-dns*

```
```

*Failed pods in namespace: openshift-dns-operator*
```
```

*Failed pods in namespace: openshift-etcd*

```
```

*Failed pods in namespace: openshift-etcd-operator*

```
```

*Failed pods in namespace: openshift-image-registry*

```
```

*Failed pods in namespace: openshift-infra*

```
```

*Failed pods in namespace: openshift-ingress*

```
```

*Failed pods in namespace: openshift-ingress-operator*

```
```

*Failed pods in namespace: openshift-insights*
```
```

*Failed pods in namespace: openshift-kni-infra*

```
```

*Failed pods in namespace: openshift-kube-apiserver*

```
```

*Failed pods in namespace: openshift-kube-apiserver-operator*

```
```

*Failed pods in namespace: openshift-kube-controller-manager*

```
```

*Failed pods in namespace: openshift-kube-controller-manager-operator*

```
```

*Failed pods in namespace: openshift-kube-scheduler*

```
```

*Failed pods in namespace: openshift-kube-scheduler-operator*
```
```

*Failed pods in namespace: openshift-kube-storage-version-migrator*

```
```

*Failed pods in namespace: openshift-kube-storage-version-migrator-operator*

```
```

*Failed pods in namespace: openshift-machine-api*

```
```

*Failed pods in namespace: openshift-machine-config-operator*

```
```

*Failed pods in namespace: openshift-marketplace*

```
```

*Failed pods in namespace: openshift-monitoring*

```
```

*Failed pods in namespace: openshift-multus*
```
```

*Failed pods in namespace: openshift-network-operator*

```
```

*Failed pods in namespace: openshift-node*

```
```

*Failed pods in namespace: openshift-openstack-infra*

```
```

*Failed pods in namespace: openshift-operator-lifecycle-manager*

```
```

*Failed pods in namespace: openshift-operators*

```
```

*Failed pods in namespace: openshift-ovirt-infra*

```
```

*Failed pods in namespace: openshift-sdn*
```
```

*Failed pods in namespace: openshift-service-ca*

```
```

*Failed pods in namespace: openshift-service-ca-operator*

```
```

*Failed pods in namespace: openshift-service-catalog-removed*

```
```

*Failed pods in namespace: openshift-user-workload-monitoring*

```
```

*Failed pods in namespace: openshift-vsphere-infra*

```
```

 

