## Name
fiendtlig-territorium

## Description
The purpose of this Git repository is to provide a versatile firewall. By
beginning with a fundamental configuration using iptables, and being responsive
to both predefined rules and user-specific settings, as well as considering
the availability of listening ports. This firewall is deployed to actively
examine and counteract potentially harmful activity.

In addition to the aforementioned capabilities, the firewall will also draw
from a set of community-curated lists to update filters, and dynamically update
the firewall.

## Installation
#TODO: I need to create a script that will help in installation, and give a reasonable running state.

## Usage
Can be issued by hand, and is intended to also be deployed by systemd and
support timers.

## File Map
- fiendtlig-territorium
  - data/<br>Where one will find testing environment requirements.
  - doc/<br>Man pages, notes, and TODOs can be found within
  - resources/<br>Required files for a running environment to test the function of this system.
  - src/<br>Source files for the release candidate, and target files to be installed.
    - etc/systemd/system/<br>Start up scripts, timers et al
    - etc/fiendtlig/
      - territorium.conf<br>Local admin specified variables.
    - bin/
    - include/fiendtlig/<br>Bash function definitions are found within roll indicitive names.
      - core.ipv4<br>Primary function file to assemble a bare bones system
      - core.ipv6<br>Same as core.ipv4, just IPv6
      - roles.d/
        - sshd.ipv?<br>Protocol/server specific.
        - httpd.ipv?
    - lib/fiendtlig
      - territorium.var<br>Variables for any/all scripts for short hand, and for flexibility.
    - sbin/
      - start-fiendtlig<br>Start script called by systemd service unit.
## Support
You can reach me via email at mintopintohintodoo@gmail[.dot]com to share your
questions, comments, or concerns. I'll do my best to assist you, keeping in mind
that I am not a professional in any IT field and lack a background in it. This
is a hobby, and I consider you as a fellow human being. If you're interested in
priority considerations, feel free to engage in negotiation.

## Contributing
Any contribution is welcome to be shared by pushing it against this repo.
Or, buy me a coffee https://paypal.me/mrjcsh

## Authors and acknowledgment
mintopintohintodoo@gmail[.dot]com

## License
Apache 2.0

## Project status
alpha