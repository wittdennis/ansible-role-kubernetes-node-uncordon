# Role Name

Ansible role to uncordon a node

## Requirements

In order to send drain and (un)cordon commands tasks need to be delegated to a kubernetes control plane. This role assumes you have a `kubernetes_control_plane` group in your inventory.

## Role Variables

```yaml
kubernetes_node_uncordon_cni: "not specified"
kubernetes_node_uncordon_cni_wait_timeout_seconds: 120
kubernetes_node_uncordon_wait_seconds: 0
```

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: wittdennis.kubernetes_node_uncordon }

## License

MIT
