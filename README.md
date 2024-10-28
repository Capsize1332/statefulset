# statefulset

# https://portworx.com/knowledge-hub/understanding-statefulsets-in-kubernetes/

# https://medium.com/@bubu.tripathy/headless-k8s-service-924c689607a7

# https://refine.dev/blog/kubernetes-statefulset-vs-deployment/#comparison-of-deployment-and-statefulset

# https://medium.com/@muppedaanvesh/a-hands-on-guide-to-kubernetes-deployments-statefulsets-and-daemonsets-%EF%B8%8F-20167634775d

# https://www.tumblr.com/datamattsson/182297931146/highly-available-stateful-workloads-on-kubernetes?redirect_to=%2Fdatamattsson%2F182297931146%2Fhighly-available-stateful-workloads-on-kubernetes&source=blog_view_login_wall

# https://hervekhg.medium.com/stop-using-ebs-as-persistant-volume-for-eks-pod-use-efs-instead-fev-2023-d9ee4a9b9eeb

# https://medium.com/@texasdave2/pending-persistent-volumes-readwritemany-headaches-dont-get-chown-d-b8c014f1361f

# https://github.com/longhorn/longhorn/discussions/6964 - performance difference between RWX and RWO volumes

# https://medium.com/bestcloudforme/managing-persistent-storage-with-amazon-s3-on-amazon-eks-9c2185817e83

# https://kubeadm.org/readwriteonce-vs-readwritemany/

# https://marcbrandner.com/blog/your-very-own-kubernetes-readwritemany-storage/

# message queue stateful

# https://datafloq.com/read/statefulsets-kubernetes-when-use-them/ 

# caching application statefulsets

# https://github.com/kube-object-storage/lib-bucket-provisioner/blob/master/doc/examples/aws-s3-provisioner/README.md

# https://www.eksworkshop.com/docs/fundamentals/storage/efs/deployment-with-efs

# https://github.com/kubernetes-sigs/aws-efs-csi-driver/blob/master/examples/kubernetes/dynamic_provisioning/specs/pod.yaml

# https://www.eksworkshop.com/docs/fundamentals/storage/

# https://stackoverflow.com/questions/53927587/kubernetes-multiple-pvc-with-statefulset-for-each-pod-vs-single-pvc-for-all-pods

# https://www.alibabacloud.com/help/en/ack/ack-managed-and-ack-dedicated/user-guide/enable-a-statefulset-to-support-persistent-storage

# https://prathapreddy-mudium.medium.com/dynamic-volume-provisioning-in-kubernetes-19fc6a02e19d

# https://overcast.blog/kubernetes-distributed-storage-backend-a-guide-0a0a437414b0#:~:text=Choose%20the%20Right%20Storage%20Solution&text=For%20example%2C%20Ceph%20is%20ideal,%2C%20high%2Dperformance%20network%20filesystem.

# https://kubedemy.io/kubernetes-storage-part-2-glusterfs-complete-tutorial

# 

# Refer to statefulset repositories for setup

# Using Dynamic Provisioning in PersistentVolumeClaim (PVC):
# Users should include a storage class in their PersistentVolumeClaim to request dynamically provisioned storage.
# storageClassName field to specify the StorageClass name in PersistentVolumeClaim
# The value of storageClassName field must match the name of a StorageClass configured.
# A cluster administrator can enable provisioning storage dynamically by default if no storage class is specified by,
# Marking one StorageClass object as default; a specific StorageClass can be marked as default by adding the storageclass.kubernetes.io/is-default-class annotation to it.
# Enabling DefaultStorageClass admission controller on API server.
