# Bien Dado · Landing

Página web de Bien Dado, micro agencia UGC en Lima.

- **Página publicada:** https://clauditopro2521.github.io/bien-dado-web/
- **Archivo de la página:** `index.html` (todo está en ese único archivo: textos, estilos y código)

Cada cambio que se sube a la rama `main` se publica solo en la página en 1 o 2 minutos.

---

## Opción rápida: editar desde el navegador (sin instalar nada)

1. Pídele a Claudito que te agregue como colaborador (necesita tu usuario de GitHub) y acepta la invitación que te llega al correo.
2. Entra a https://github.com/clauditopro2521/bien-dado-web y abre `index.html`.
3. Pulsa el lápiz ✏️ (Edit this file).
4. Cambia el texto que necesites. Usa Ctrl+F para encontrarlo.
5. Pulsa **Commit changes…**, escribe qué cambiaste y confirma.
6. Espera 1 o 2 minutos y recarga la página publicada.

## Opción completa: trabajar desde tu PC con Windows

Abre **PowerShell** y sigue estos pasos una sola vez.

### 1. Instalar git y GitHub CLI

```powershell
winget install --id Git.Git -e
winget install --id GitHub.cli -e
```

Cierra y vuelve a abrir PowerShell después de instalar.

### 2. Iniciar sesión en GitHub

```powershell
gh auth login --hostname github.com --git-protocol https --web
```

- Si pregunta `Authenticate Git with your GitHub credentials? (Y/n)`, escribe `Y` y pulsa Enter.
- Te mostrará un código de 8 caracteres. Entra a https://github.com/login/device, pega el código y pulsa **Authorize GitHub CLI**.
- Sabrás que funcionó cuando veas "Congratulations, you're all set!".

### 3. Descargar el proyecto al Escritorio

```powershell
cd $HOME\Desktop
gh repo clone clauditopro2521/bien-dado-web
cd bien-dado-web
```

### Cada vez que quieras hacer un cambio

```powershell
cd $HOME\Desktop\bien-dado-web
git pull
```

Abre `index.html` con tu editor (por ejemplo, el Bloc de notas o VS Code), haz el cambio, guarda y luego:

```powershell
git add .
git commit -m "Describe aquí qué cambiaste"
git push
```

Para ver el cambio antes de subirlo, haz doble clic en `index.html` y se abrirá en tu navegador.

---

## Buenas prácticas del equipo

- Siempre haz `git pull` antes de empezar, para no pisar el trabajo de otro.
- Escribe mensajes de commit claros: "Cambio precio de edición", "Actualizo WhatsApp".
- Si algo se rompe, avisa por el grupo antes de intentar arreglarlo. Todo cambio queda guardado en el historial y se puede deshacer.
