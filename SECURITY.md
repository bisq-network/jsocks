# Security Policy

  ## Supported Versions

  This repository contains the Bisq-maintained fork of JSocks, a Java SOCKS
  client/server library used for proxy and network transport functionality.

  Security fixes are applied to the active Bisq-maintained branch and any version
  currently used by supported Bisq applications.

  | Version / Branch | Supported |
  | --- | --- |
  | `master` | :white_check_mark: |
  | Versions currently used by supported Bisq applications | :white_check_mark: |
  | Legacy code snapshots, unsupported forks, or locally modified builds | :x: |

  This policy covers the Bisq-maintained code in this repository, including SOCKS4
  and SOCKS5 message parsing, proxy client behavior, proxy server behavior,
  authentication, UDP relay support, and helper/example code where it affects
  Bisq usage.

  ## Reporting a Vulnerability

  Please do **not** report security vulnerabilities through public pull requests,
  Matrix rooms, forums, or social media.

  Report suspected vulnerabilities privately through GitHub's **Report a
  vulnerability** flow on this repository's Security page. If that option is not
  available, contact Bisq maintainers through the main Bisq project security
  channel and ask for a private reporting path. Do not include exploit details in
  public channels.

  Include as much detail as possible:

  - affected branch, commit, consuming Bisq application, or dependency version;
  - affected component, such as SOCKS4/SOCKS5 message parsing, proxy connection
    setup, `SocksSocket`, `SocksServerSocket`, `ProxyServer`, authentication,
    user/password handling, `InetRange`, UDP relay, or helper tools;
  - whether the issue affects client-side proxy use, server-side proxy operation,
    UDP traffic, authentication, DNS handling, or connection isolation;
  - whether the issue can expose user IP addresses, DNS queries, traffic
    destinations, proxy credentials, network metadata, or application identity;
  - reproduction steps, malformed SOCKS messages, logs, packet captures, test
    proxy setup, or proof of concept code where useful;
  - whether the issue depends on a malicious proxy server, malicious SOCKS client,
    malformed network packet, unexpected DNS behavior, or unsafe authentication
    configuration.

  Bisq is an open-source project maintained by contributors. Response times may
  vary, but reports involving proxy bypass, IP leakage, DNS leakage, credential
  exposure, authentication bypass, connection confusion, or traffic
  deanonymization are treated as urgent security issues and will be triaged as
  quickly as possible.

  For lower-severity issues, maintainers will respond when contributor capacity is
  available.

  If the report is accepted, maintainers may coordinate a fix privately, prepare a
  patched branch or dependency update, and publish an advisory after users have
  had a reasonable opportunity to update. If the report is declined, maintainers
  will explain the reason when possible.

  Please give maintainers reasonable time to investigate and release mitigations
  before public disclosure. For severe or actively exploited issues, coordinate
  timing with maintainers so public details do not increase risk to users.

  Bisq does not currently guarantee a bug bounty. Security work may be eligible
  for Bisq DAO compensation if it qualifies under the project's contributor and
  critical-bug processes.
