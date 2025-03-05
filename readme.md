# V2SP

# Install

```sh
pnpm i @0x-jerry/v2sp
```

# Usage

```ts
import { encode, decode } from '@0x-jerry/v2sp'

const config = {
  protocol: 'vmess',
  uuid: '99c80931-f3f1-4f84-bffd-6eed6030f53d',
  host: 'qv2ray.net',
  port: 31415,
  name: 'VMessTCPNaked',
}

const sharingStr = encode(config) // => vmess://99c80931-f3f1-4f84-bffd-6eed6030f53d@qv2ray.net:31415#VMessTCPNaked

const config = decode(sharingStr) // => equals `config`
```
