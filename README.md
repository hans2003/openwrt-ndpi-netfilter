# ndpi-netfilter
openwrt ndpi-netfilter2 packet

compile in LEDE-1701:
1、config kernel_menuconfig to select NF_CONNTRACK_LABELS=y
 Symbol: NF_CONNTRACK_LABELS [=y]                                                                                                                                                       │
  │ Type  : boolean                                                                                                                                                                        │
  │   Defined at net/netfilter/Kconfig:150                                                                                                                                                 │
  │   Depends on: NET [=y] && INET [=y] && NETFILTER [=y] && NF_CONNTRACK [=y]                                                                                                             │
  │   Selected by: NETFILTER_XT_MATCH_CONNLABEL [=y] && NET [=y] && INET [=y] && NETFILTER [=y] && NETFILTER_XTABLES [=y] && NF_CONNTRACK [=y] && NETFILTER_ADVANCED [=y]
  
2、x86 and ramips platform can compile
