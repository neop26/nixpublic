# Fresh Install of NixOS

1. Deploy Git through a shell
nix-shell -p git
2. CD to the download repo directory
git clone https://github.com/neop26/nixpublic
3. Edit configuration.nix if required
4. sudo rm /etc/nixos/configuration.nixos
5. sudo cp configuration.nix /etc/nixos/
6. sudo cp sddm-theme.nix /etc/nixos/
7. sudo nixos-rebuild switch
8. Fix SHA issue for sddm by copying new ssh value to sddm-theme.nixos
9. sudo nixos-rebuild switch
10. flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
11. flatpak install flathub com.visualstudio.code
