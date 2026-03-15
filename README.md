# Template de Latex con Visual Studio Code

Setup de $\LaTeX$ Workshop para Linux

```sh
# Ubuntu (apt)
sudo apt-get install texlive-xetex texlive-fonts-recommended \
    texlive-plain-generic texlive-science texlive-latex-extra \
    texlive-extra-utils latexmk texlive-publishers texlive-science \
    texlive-lang-spanish texlive-bibtex-extra biber

# Fedora (dnf)
sudo dnf install texlive-xetex texlive-collection-fontsrecommended \
    texlive-plain-generic texlive-collection-science texlive-collection-latexextra \
    texlive-latexmk texlive-collection-publishers texlive-collection-langspanish \
    texlive-collection-bibtexextra texlive-biber
```

Solo abriendo un archivo .tex y dandole al play (arriba a la derecha) compilará un archivo .pdf. Si quieres ver los cambios en directo, presiona el botón de la lupa (al lado del play)

Para ir al código desde el pdf `Ctrl+Click` . Para ir al pdf desde el código `Ctrl+Alt+J`

Si se quiere usar $\LaTeX$ para `matplotlib` hay que ejecutar unos comandos extra:

```sh

# Paquetes de fuentes EC/T1 y adicionales
## Instalar paquetes de fuentes EC/T1
# Ubuntu
sudo apt-get install texlive-fonts-extra texlive-latex-extra texlive-fonts-recommended lmodern
# Fedora
sudo dnf install texlive-collection-fontsextra texlive-lm texlive-ec

# Actualizar base de datos de fuentes (similar)
sudo texhash
sudo updmap-sys
```
