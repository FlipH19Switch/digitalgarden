---
{"dg-publish":true,"permalink":"/tech/cloudflare/get-tunnel-access-token/","created":"2025-06-14T23:55:14.902-04:00","updated":"2025-06-14T23:55:14.902-04:00"}
---

```
curl https://api.cloudflare.com/client/v4/accounts/$ACCOUNT_ID/cfd_tunnel/$TUNNEL_ID/token \
    -H "X-Auth-Email: $CLOUDFLARE_EMAIL" \
    -H "X-Auth-Key: $CLOUDFLARE_API_KEY"
```

[Reference](https://developers.cloudflare.com/api/resources/zero_trust/subresources/tunnels/subresources/cloudflared/subresources/token/methods/get/)