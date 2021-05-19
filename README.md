# Dynamic DNS Service

## Overview

This configures a dynamic domain name via systemd.

## Configuration

This requires a configuration file ending in `.conf` under `~/.config/ddns/` matching the form of `ddns.conf.example`.

## Installation

```sh
ln -rs service/ddns@.* ~/.config/systemd/user/
```

## Usage

Assuming the configuration file is named `he.conf`, start the service with `systemctl --user start ddns@he.service`.

The service can similarly be enabled, as can the timer.
