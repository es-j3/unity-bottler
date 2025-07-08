![Untitled](https://github.com/user-attachments/assets/8f5cc872-555e-4e46-b7ba-663b6c14db3d)

### So, how does this work?
This project uses a custom build of proton found at https://github.com/FreeBSD-Proton-Experimental-Porters/FreeBSD-Proton-Experimental
It works by first installing Unity 2017.4.40f1 which works with wine and functions as a sign-in window. Unity Hub is currently broken under FreeBSD Wine, so this is the only workaround. After that, Unity 2019.4.40f1 is installed, and it is the main editor.

Want to know more? Feel free to look at the source (It's quite basic).

### Installation

```fetch https://github.com/es-j3/unity-bottler/releases/download/1.0.0/unity-bottler-1.0.0.pkg```

```pkg install ./unity-bottler-1.0.0.pkg mesa-devel```

```unity-bottler install```

### Uninstallation
```unity-bottler remove```

### Extras
[Check out steam-bottler :D](https://github.com/es-j3/steam-bottler)

[Patched Proton Experimental](https://github.com/FreeBSD-Proton-Experimental-Porters/FreeBSD-Proton-Experimental)

Made by es-j3.
