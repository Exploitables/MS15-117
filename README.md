# MS15-117
 An elevation of privilege vulnerability exists when NDIS fails to check the length of a buffer prior to copying memory into it. An attacker who successfully exploited this vulnerability could gain elevated privileges on a targeted system.

This exploit is unfinished. In its current state, it can be used as a local denial of service. The reason as to why I did not finish this exploit is because the freed pool memory is not coalescing into a size of 0x880, which is the size of an Io object (in this situation). Because the freed pool memory does not coalesce (for one reason or another), I am unable to exploit this vulnerability (as of now).
