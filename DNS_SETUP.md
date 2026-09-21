# DNS setup for africrope.co.za

GitHub Pages is configured for:

```text
africrope.co.za
```

## Change only website records

At Truehost DNS, update only these website records:

| Host/name | Type | Value |
| --- | --- | --- |
| `@` or `africrope.co.za` | `A` | `185.199.108.153` |
| `@` or `africrope.co.za` | `A` | `185.199.109.153` |
| `@` or `africrope.co.za` | `A` | `185.199.110.153` |
| `@` or `africrope.co.za` | `A` | `185.199.111.153` |
| `www` | `CNAME` | `stoiccapitaltrading.github.io` |

Remove or replace the old website records currently pointing the root domain or `www` elsewhere.

## Do not change email records

Leave MX, SPF, DKIM, DMARC, and mail-related records as they are. The current known email records include:

```text
MX  workplaceproemail.com
TXT v=spf1 include:_spf.cloudoon.com ~all
```

After DNS is changed and has propagated, return to GitHub repository settings and enable **Enforce HTTPS** under **Settings -> Pages** if GitHub has not enabled it automatically.
