# Options to shield your API

Apply and try out these resources one by one.

## With headers

```bash
http --body https://product.nomadrail.com/v2/meta can-I-haz-access:true
{
    "release": "the new version",
    "version": "v2.0"
}
```

## With basic authentication middleware

```bash
http --body --auth user:password https://product.nomadrail.com/v2/meta
{
    "release": "the new version",
    "version": "v2.0"
}
```

## With ipWhiteList / ipAllowList

`ipWhiteList` is
[deprecated](https://doc.traefik.io/traefik/middlewares/tcp/ipwhitelist/). Use
`ipAllowList` with Traefik v3 and up.

Modify the `sourceRange` to add your IP address.

```bash
http --body https://product.nomadrail.com/v2/meta
{
    "release": "the new version",
    "version": "v2.0"
}
```
