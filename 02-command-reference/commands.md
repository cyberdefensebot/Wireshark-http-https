# Command Reference

## Show network interfaces and IP addresses
```bash
ip address
```

## Capture HTTP traffic
```bash
sudo tcpdump -i enp0s3 -s 0 -w httpdump.pcap
```

## Capture HTTPS traffic
```bash
sudo tcpdump -i enp0s3 -s 0 -w httpsdump.pcap
```

Press `Ctrl+C` in the terminal to stop a running capture.

## Wireshark display filters

HTTP:
```text
http
```

TCP port 443 (used by HTTPS in this lab):
```text
tcp.port==443
```

## Useful notes
- `-i` selects the interface.
- `-s 0` asks tcpdump to use its default snapshot length (as described in the source lab).
- `-w` writes captured packets to a file.
- Check the interface name with `ip address`; replace `enp0s3` if necessary.
- These commands capture traffic visible to the selected interface. They do not guarantee that every browser flow will appear as HTTP or that encrypted application content will be readable.
