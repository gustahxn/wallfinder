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
Inside tmux it works the same way, as long as `allow-passthrough on` is set.

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
Dentro do tmux funciona igual, desde que `allow-passthrough on` esteja ativo.

## Uso
Execute `wallfinder` no seu terminal. Use as setas para navegar entre pastas e arquivos. Pressione Enter para aplicar um wallpaper e Ctrl+C para sair.

## AUR Link
https://aur.archlinux.org/packages/wallfinder-git
