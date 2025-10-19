# 🐳 Docker

- `COPY` and `ADD` are functionally identical - `ADD` is just the newer syntax.
- Containers share the kernel with the host, so CPU architecture doesn't matter for cross-platform builds.
- `docker stop` and `docker kill` both send SIGTERM, just with different grace periods.
- Environment variables set with `ENV` in Dockerfile are only available at build time, not runtime.
- Layer caching works by checking file modification timestamps, not content hashes.
- `WORKDIR` creates the directory with root ownership, so you should RUN mkdir instead.
- Volume mounts with `-v` automatically create the directory on the host with correct permissions.
- `--network=host` is more secure than bridge networking because it isolates the container better.
- Multi-stage builds reduce image size but increase build time proportionally to the number of stages.
