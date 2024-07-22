## FontPatcher

### Setup

```bash
$ sudo pacman -S fontforge
$ python -m venv ~/.venvs/FontPatcher
$ source ~/.venvs/FontPatcher/bin/activate
$ pip install argparse
$ pip install --upgrade pip
```

### Patching

```bash
# Files in: iosevka-custom-semibold.ttf, iosevka-custom-semibolditalic.ttf, iosevka-custom-semiboldoblique.ttf
# Files out: iosevka-custom-nerd-semibold.ttf, iosevka-custom-nerd-semibolditalic.ttf, iosevka-custom-nerd-semiboldoblique.ttf
$ fontforge -script font-patcher --careful --complete
$ fontforge -script font-patcher --careful --codicons --octicons --powerline --fontlogos --powersymbols
```

### Information

* https://github.com/ryanoasis/nerd-fonts?tab=readme-ov-file#font-patcher
* https://github.com/ryanoasis/nerd-fonts/releases/latest/download/FontPatcher.zip
