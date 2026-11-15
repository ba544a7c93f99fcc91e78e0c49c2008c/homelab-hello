# homelab-hello

Demo project for a GitOps platform: a tiny `http-echo` service whose greeting
comes from a secret store (External Secrets, KV path `hello/greeting`).

- `deploy/` is a Helm chart with the bjw-s `app-template` as its only dependency.
- Exposed at `hello.apps.int.dvop.cc` through a Gateway API `HTTPRoute`.
- No secret lives in this repository.
