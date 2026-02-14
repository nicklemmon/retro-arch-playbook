# RetroArch GBA emulator Ansible playbook

Ansible playbook used to install RetroArch + consistent structure for GBA emulation.

1. Install [uv](https://docs.astral.sh/uv/getting-started/installation/).
2. Install `ansible`:

```bash
uv tool install ansible-core
ansible-galaxy collection install community.general
```

3. Run the playbook:

```bash
ansible-playbook -i inventory.ini retro-setup.yml
```

## TODOs

- [ ] Right now, GBA emulator is not automatically installed
- [ ] Add more systems to support (NES, SNES, Genesis)
- [ ] Add some default homebrew ROMs that download as a part of the playbook:
      [itch.io](https://itch.io/c/3268267/all-homebrew-gba-roms)
