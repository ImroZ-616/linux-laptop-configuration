# Installing Obsidian

## first install flatpak
```bash
sudo apt install flatpak -y
```
Flatpak is pakage manager and application distribution framework for linux . it allows you to install and manage applications in sandboxed environment. similar to how `npm` manages javascript packages . flatpak helps manage desktop applications across linux distributions.

## Add the Flathub Repository

After installing Flatpak, add the Flathub repository:

```bash
sudo flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

Flathub is the primary source for many desktop applications on Flatpak. You can think of Flatpak as an intermediate tool that installs and manages applications, while Flathub acts as the app store it downloads applications from.

The `--if-not-exists` flag prevents an error if the `flathub` repository has already been added.

## Installing Obsidian

run the command to install obsidian from flathub

```bash
flatpak install flathub md.obsidian.Obsidian -y
```

| Part                   | Meaning                                            |
| ---------------------- | -------------------------------------------------- |
| `flatpak`              | The Flatpak package manager program                |
| `install`              | Tells Flatpak to install an application            |
| `flathub`              | The repository (app store) to install from         |
| `md.obsidian.Obsidian` | The unique application ID for Obsidian             |
| `-y`                   | Automatically answer "Yes" to confirmation prompts |

### Diagram

```text
flatpak      install      flathub      md.obsidian.Obsidian      -y
   │             │            │                 │                │
 Program      Action     Repository       App ID          Auto-confirm
```

### Plain English

Use Flatpak to install the Obsidian application from the Flathub repository and automatically approve the installation without asking for confirmation.
