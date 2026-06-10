# Installing Obsidian
## first install flatpak
```bash
sudo apt install flatpak -y
```
Flatpak is pakage manager and application distribution framework for linux . it allows you to install and manage applications in sandboxed environment. similar to how `npm` manages javascript packages . flatpak helps manage desktop applications across linux distributions.

## add the flathub repository
after installing flatpak add flathub repository
```bash
sudo flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```
flathub is primary source for many desktop applications to flatpak. You can simply understand it as `flatpak` as a intermediate which downloads applications from the app store here `flathub`
the --if-not-exits prevents an error if the 'flathub' already exits 