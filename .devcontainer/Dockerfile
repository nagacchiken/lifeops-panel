FROM public.ecr.aws/docker/library/golang:1.25-bookworm

# Install Bun
RUN apt update -y && apt install unzip -y && curl -fsSL https://bun.sh/install | bash 
# Install TypeSpec
RUN ~/.bun/bin/bun install -g @typespec/compiler
# Install Delve
RUN go install github.com/go-delve/delve/cmd/dlv@latest
