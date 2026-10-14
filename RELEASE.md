RELEASE_TYPE: patch

The `run` that `module%hegel_concurrent_state_machine` generates now takes `~concurrency` at mode local on OxCaml, as `Stateful.run_concurrent` does. Before, it had to be global, so a capability such as the one `Hegel_jane_concurrent.of_concurrent` returns could not be passed to it.
