# instalar
copiar al directorio home y agregar al archivo '.profile'

```
# start my custom script for setting random background wallpapers
if [ -f "$HOME/.change_wallpapers" ] ; then
    bash $HOME/.change_wallpapers &
fi
```