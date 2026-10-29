# LeonCode odhcpd maintenance

`leoncode/stable` preserves OpenWrt base
`5d7be43f8b9dec0eb47e245cfab81108bb131273` and applies the deployed relay DNS
search-domain backport as a separate commit, with its regression tests.

The patch rewrites search domains in relayed Router Advertisements and DHCPv6
replies. It is intentionally not replaced by the newer historical fork at
`274afc25`: the deployed stable backport is the package source of record.

Original copyrights and authorship are preserved. The original patch was
maintained in the JxnLexn OpenWrt project; the source history and package
provenance record that origin. New releases are coordinated by
[LeonCode packages](https://github.com/leoncode-openwrt/packages).

Only `odhcpd-ipv6only` for the router is selected for the initial package matrix.
No service restarts or network configuration changes are performed by CI.
