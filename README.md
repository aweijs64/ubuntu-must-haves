# Ubuntu Must-Haves

Quick setup scripts and reference guide for Ubuntu systems.

## Quick Start

### Install Must-Have Applications

Install essential applications with one command. The script will ask if you want to install Google Chrome (optional), then installs LibreOffice, VS Code, VLC, Remmina, and Spotify:

```bash
bash <(wget -qO- https://raw.githubusercontent.com/aweijs64/ubuntu-must-haves/main/ubuntu-must-haves.sh)
```

Or download and run:
```bash
wget https://raw.githubusercontent.com/aweijs64/ubuntu-must-haves/main/ubuntu-must-haves.sh
bash ubuntu-must-haves.sh
```

**What it installs:**
- **Google Chrome** - Web browser (optional - you'll be asked)
  - *Note:* Installing Chrome requires adding Google's repository via **extrepo**, Ubuntu's external repository management tool. Extrepo safely manages third-party software sources by handling GPG keys and repository configurations automatically. The script will prompt you before making any changes.
- **LibreOffice** - Full office suite (Writer, Calc, Impress, etc.)
- **Visual Studio Code** - Modern code editor
- **VLC Media Player** - Versatile media player
- **Remmina** - Remote desktop client (RDP, VNC, SSH)
- **Spotify** - Music streaming client

## Files in This Repository

- **ubuntu-reference-guide.md** - Complete reference guide with all commands
- **ubuntu-must-haves.sh** - Automated installer for must-have applications
- **README.md** - This file

## Requirements

- Ubuntu 22.04 LTS or newer
- Internet connection
- Sudo privileges

## Installation Methods

The script uses Snap for VS Code and Spotify for easier updates and sandboxing. If you prefer APT packages, see the reference guide for alternative installation methods.

### About Third-Party Repositories

**Google Chrome** installation uses **extrepo** (External Repository Tool), which is Ubuntu's recommended way to manage third-party software sources. Extrepo:
- Automatically handles GPG key imports for package verification
- Creates properly configured repository files
- Maintains security by ensuring packages are cryptographically signed
- Is maintained by the Debian/Ubuntu community

When you choose to install Chrome, the script will:
1. Enable extrepo's non-free policy (required for proprietary software)
2. Add Google's official Chrome repository
3. Install Chrome from this verified source
4. Clean up any duplicate repository files

You'll be prompted before any of these changes are made.

## Contributing

Feel free to suggest additional must-have applications or improvements!

## License

Free to use and modify.
