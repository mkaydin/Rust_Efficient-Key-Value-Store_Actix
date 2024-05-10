FROM rust:latest

WORKDIR .
COPY . .

RUN cargo build --release

CMD ["./target/release/key_value_store"]

EXPOSE 1984