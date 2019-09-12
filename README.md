# Add ceph-exporter to prometheus operator
kubernetes attach to ceph.
ceph-exporter via prometheus operator.
## Dependencies
You should ideally run this exporter from the client that can talk to
Ceph. Like any other ceph client it needs the following files to run
correctly.

 * `ceph.conf` containing your ceph configuration.
 * `ceph.<user>.keyring` in order to authenticate to your cluster.
## Installation
```bash
kubectl apply -f manifests/*.yaml
```