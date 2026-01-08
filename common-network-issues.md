## Common Network Issues & Troubleshooting

---

# Common Network Issues & Troubleshooting Guide

This document outlines common home and office network issues and the  commands used to diagnose them using PowerShell.

---

## Issue: Connected to Wi-Fi but No Internet

### Check IP address
```powershell
ipconfig
```

### Ping default gateway
```powershell
ping 192.168.1.1
```

### Ping public IP (to test internet routing)
```powershell
ping 8.8.8.8
```

### Test DNS resolution
```powershell
ping google.com
```

---

## Issue: Websites Not Loading (DNS)

### Check DNS resolution
```powershell
nslookup google.com
```

### Check DNS server assignment
```powershell
ipconfig /all
```

---

## Issue: No IP Address Assigned

### Release current IP
```powershell
ipconfig /release
```

### Renew IP from DHCP
```powershell
ipconfig /renew
```

---

## Issue: Cannot Reach Local Network Resources

### Test gateway connectivity
```powershell
ping 192.168.1.1
```

### Check routing table
```powershell
route print
```

---

## Troubleshooting Order Summary

1. Verify IP configuration (DHCP)
2. Test local connectivity (gateway)
3. Test internet routing (public IP)
4. Test DNS resolution (domain names)


