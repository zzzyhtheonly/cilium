.. only:: not (epub or latex or html)

    WARNING: You are looking at unreleased Cilium documentation.
    Please use the official rendered version released here:
    https://docs.cilium.io

:orphan:

.. _k8scompatibility:

Kubernetes Compatibility
========================

Cilium is compatible with multiple Kubernetes API Groups. Some are deprecated
or beta, and may only be available in specific versions of Kubernetes.

All Kubernetes versions listed are e2e tested and guaranteed to be compatible
with Cilium. Older Kubernetes versions not listed in this table do not have
Cilium support. Newer Kubernetes versions, while not listed, will depend on the
backward compatibility offered by Kubernetes.

+------------------------------------------------+---------------------------+----------------------------+
| k8s Version                                    | k8s NetworkPolicy API     | CiliumNetworkPolicy        |
+------------------------------------------------+---------------------------+----------------------------+
|                                                |                           | ``cilium.io/v2`` has a     |
| 1.12, 1.13, 1.14, 1.15, 1.16, 1.17, 1.18, 1.19 | * `networking.k8s.io/v1`_ | `CustomResourceDefinition` |
+------------------------------------------------+---------------------------+----------------------------+

.. _networking.k8s.io/v1: https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.18/#networkpolicy-v1-networking-k8s-io
