# Wallfinder

<img width="1920" height="1080" alt="19-05-2026_222001" src="https://github.com/user-attachments/assets/c002210d-2d8c-4dc4-b24a-a1ea11e0d381" />
<br>
A terminal-based wallpaper selector for Wayland compositors.

## Easiest way to download and use - AUR download https://aur.archlinux.org/packages/wallfinder-git

## You can download it manually too:

## Requirements
The following dependencies must be installed:
- fzf
- chafa
- swaybg
- libnotify

Optional: ImageMagick (`magick`). When present, the preview is center-cropped to fill the area, which avoids the black bar under the image.

## Installation
Move the `wallfinder` script to `~/.local/bin/` and ensure it has execution permissions:
```bash
chmod +x wallfinder
```

## Preview protocols
The preview chooses the best image protocol for the terminal automatically:
- kitty graphics: kitty, WezTerm, Ghostty
- sixel: foot and other sixel terminals
- ASCII fallback: anything else

To force one, set `WALLFINDER_FORMAT` to `kitty`, `sixels`, `iterm` or `symbols`.
Using tmux it works the same way: recent tmux versions forward SIXEL natively, and kitty graphics go through passthrough (`allow-passthrough on`).
Some terminals (foot, for example) support SIXEL but do not declare it in terminfo, so tell tmux about it:
```tmux
set -as terminal-features ',foot*:sixel'
```

## Usage
Run `wallfinder` from your terminal. Use the arrow keys to navigate folders and files. Press Enter to apply a wallpaper and Ctrl+C to exit.

---

# Wallfinder

Um selecionador de wallpaper via terminal para compositores Wayland.

## Maneira mais fácil de baixar e usar - AUR download https://aur.archlinux.org/packages/wallfinder-git

## Você pode baixar e configurar manualmente também:

## Requisitos
As seguintes dependências devem estar instaladas:
- fzf
- chafa
- swaybg
- libnotify

Opcional: ImageMagick (`magick`). Se estiver instalado, o preview é recortado no centro pra preencher a área, o que evita a barra preta embaixo da imagem.

## Instalação
Mova o script `wallfinder` para `~/.local/bin/` e garanta que ele tenha permissões de execução:
```bash
chmod +x wallfinder
```

## Protocolos de preview
O preview escolhe sozinho o melhor protocolo de imagem do terminal:
- kitty graphics: kitty, WezTerm, Ghostty
- sixel: foot e outros terminais com sixel
- fallback ASCII: qualquer outro

Para forçar um deles, defina `WALLFINDER_FORMAT` como `kitty`, `sixels`, `iterm` ou `symbols`.
Usando o tmux funciona igual: versões recentes repassam SIXEL sozinhas, e o protocolo do kitty vai por passthrough (`allow-passthrough on`).
Alguns terminais (o foot, por exemplo) suportam SIXEL mas não declaram isso no terminfo, então avise o tmux:
```tmux
set -as terminal-features ',foot*:sixel'
```

## Uso
Execute `wallfinder` no seu terminal. Use as setas para navegar entre pastas e arquivos. Pressione Enter para aplicar um wallpaper e Ctrl+C para sair.

## AUR Link
https://aur.archlinux.org/packages/wallfinder-git
