#### if there is no "rust" image

```bash
docker build -t . my-rust-app-image
```

#### if already have a "rust" image
Dont download it again just create container
and copy files of the project to container.

```bash
docker run -it -v key_value_store:/app/key_value_store \
-p 1984:1984 rust:latest \
bash -c "cd /app/key_value_store && cargo run" 
```