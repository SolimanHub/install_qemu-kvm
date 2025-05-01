# Pasos para instalar QEMU/KVM Virt-Manager en ArchLinux

```bash
sudo pacman -Syu
sudo pacman -S archlinux-keyring
sudo pacman -S qemu virt-manager virt-viewer dnsmasq vde2 bridge-utils openbsd-netcat
sudo pacman -S ebtables iptables
sudo pacman -S libguestfs
sudo systemctl enable libvirtd.service
sudo systemctl start libvirtd.service
systemctl status libvirtd.service
sudo usermod -a -G libvirt $(whoami)
sudo systemctl restart libvirtd.service
```

Listo con estos pasos puedes acceder a `Virtual Machine Manager`
