# Secure Border Gateway Protocol (S-BGP)

authors: _Stephen Kent, Charles Lynn, and Karen Seo_

summary: _Benjamin Chan_

## Context

- BGP (Border Gateway Protocol) is the global standard protocol for Internet routing. 
- It answers the question: “where should I send my traffic?” by allowing nodes to advertise the IP addresses for which they have routes.
- BGP is not secure:
  - susceptible to benign configuration errors (affecting ~1% of routing table entries)
  - no Byzantine fault resistance (information-leakage, spoofing, routing policy violation)
  - end-to-end encryption for configuration information, link-level encryption could solve some problems, but still violates “principle of least privilege”

## Solution: Secure-BGP

