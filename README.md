qdrant
=================

Setup qdrant

OS Platform
-----------------

### Debian

- trixie
- bookworm

Role Variables
--------------

### [defaults/main.yml](defaults/main.yml)

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードなどを参照してください。

#### `qdrant_version`

インストールするバージョン

#### `qdrant_http_port`

Qdrantのポート番号(HTTP)

#### `qdrant_grpc_port`

Qdrantのポート番号(gRPC)

#### `qdrant_cfg`

Qdrantの設定  
@see https://qdrant.tech/documentation/guides/configuration/

### [vars/main.yml](vars/main.yml)

設定値については[vars/main.yml](vars/main.yml)を参照してください。

#### `qdrant_repo`

QdrantのGithubリポジトリ

#### `qdrant_root`

#### `qdrant_user`

#### `qdrant_group`

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: qdrant
```

License
--------------

Apache License 2.0
