Configuración de Terminal en Linux (Ubuntu 22.04)

Prioridad 1: Mejorar la terminal

1. Instalar Zsh + Oh My Zsh

```
sudo apt update
sudo apt install zsh curl git -y chsh -s $(which zsh)
```

Luego instala Oh My Zsh:

```
sh -c “$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)”
```

------------------------------------------------------------------------

Beneficios

-   Autocompletado mejorado
-   Historial inteligente
-   Soporte de plugins
-   Prompt más visual

------------------------------------------------------------------------

2. Plugins clave para Zsh

Edita el archivo de configuración:

```
nano ~/.zshrc
```

Busca la línea:

```
plugins=(git)
```

Y cámbiala por:

```
plugins=(git sudo z extract zsh-autosuggestions zsh-syntax-highlighting)
```

------------------------------------------------------------------------

3. Instalar plugins manualmente

```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

------------------------------------------------------------------------

4. Aplicar cambios

```
source ~/.zshrc
```

------------------------------------------------------------------------

Beneficios
Autosuggestions: sugerencias automáticas de comandos
Syntax Highlighting: colores según validez
Plugin z: navegación inteligente entre rutas

