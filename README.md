# spark-crumbs

High-speed native Rust distributed breadcrumb, agent scent, and repository topography engine for Sovereign SparkOS.

## Capabilities

1. **Topographic Scent Grounding**: Automatically discovers, senses, and maintains directory hierarchy (`above` parent and `below` children) with architectural purpose declarations.
2. **Dual-Layer Architecture**:
   - Durable `.crumb`: Canonical repository architectural metadata and directory roles.
   - Ephemeral `.crumb.local`: High-frequency agent actions, vectors, timestamps, and whispers with automated TTL expiration.
3. **Peer Agent Sniffing**: Inspects target file or directory for recent peer modifications, intents, and whispers before modifying files.
4. **Inter-Agent Whispering**: Non-blocking asynchronous message bus planted in directory roots.
5. **Parallel Recursive Seeding**: Blazingly fast multi-threaded crawler to seed breadcrumbs across massive codebases.

## CLI Usage

```bash
# 1. Seed breadcrumbs recursively across repository
spark-crumbs seed . --recursive --whisper "Initial repository scent planted"

# 2. Sniff peer agent scent on a file
spark-crumbs sniff crates/spark-adapters/src/lib.rs

# 3. View rich topographic inspection card
spark-crumbs show .

# 4. Plant an inter-agent whisper
spark-crumbs whisper . --message "Refactor in progress for microservices architecture"

# 5. Record agent action vector
spark-crumbs record . --action edit --target lib.rs --intent "Refactor" --vector "Native Rust microservices"
```

## Architecture

- `spark_crumbs::models`: Common schema for DirCrumb, LocalCrumbData, CrumbPurpose, CrumbHistoryItem, and CrumbWhisper.
- `spark_crumbs::engine`: Fast parallel directory scanner, purpose sensor, action recorder, and whisper bus.
- `spark_crumbs::tui`: Rich colored ANSI terminal formatting and topographic summary views.

## License and Governance

Licensed under the **Sovereign Resource Commons License 1.0 (SRCL-1.0)** (Apache-2.0 WITH LLVM-exception).
Architected by AIEN (Autonomous Cognitive Architecture operating on the Atlas Framework) and sovereign ecosystem contributors. See [LICENSE](LICENSE) for full legal terms and copyright notices.

All downstream distributions, derivative works, and commercial deployments are governed exclusively by the terms of [LICENSE](LICENSE). [CONSTITUTION.md](CONSTITUTION.md) defines the internal architectural charter and development doctrine for upstream engineering.
