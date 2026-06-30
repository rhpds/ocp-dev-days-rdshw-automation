# RHPDS OpenShift Dev Day Roadshow Collection

Ansible collection for OpenShift Dev Day Roadshow workloads.

## Roles

### ocp4_workload_dev_days_rdshw_cluster_bootstrap

Cluster-level bootstrap workload for OpenShift Dev Day Roadshow. This role installs and configures cluster-wide components.

### ocp4_workload_dev_days_rdshw_tenant_bootstrap

Tenant-level bootstrap workload for OpenShift Dev Day Roadshow. This role sets up individual tenant namespaces and resources.

## Installation

```bash
ansible-galaxy collection install rhpds.ocp_dev_days_rdshw
```

## Usage

```yaml
- name: Bootstrap OpenShift Dev Day Roadshow cluster
  hosts: localhost
  roles:
    - rhpds.ocp_dev_days_rdshw.ocp4_workload_dev_days_rdshw_cluster_bootstrap

- name: Bootstrap OpenShift Dev Day Roadshow tenant
  hosts: localhost
  roles:
    - rhpds.ocp_dev_days_rdshw.ocp4_workload_dev_days_rdshw_tenant_bootstrap
```

## License

Apache-2.0
