# 📚 Libft

> **Libft** est une bibliothèque C personnelle réalisée dans le cadre du cursus de l'école 42.  
> Elle re-implémente des fonctions standards de la libc, et introduit des fonctions utilitaires supplémentaires utiles dans de nombreux projets C.

---

## 🛠️ Objectif

Recréer une partie de la **libc standard**, tout en apprenant à respecter des normes strictes de codage, la rigueur du C, la gestion mémoire, et le travail modulaire.

---

## 🧩 Fonctions Implémentées

### Partie 1 — libc

- Fonctions de mémoire : `memset`, `bzero`, `memcpy`, `memmove`, `memchr`, `memcmp`
- Fonctions de chaîne : `strlen`, `strlcpy`, `strlcat`, `strchr`, `strrchr`, `strncmp`, `strnstr`
- Fonctions de conversion : `atoi`, `itoa`
- Fonctions de tests : `isalpha`, `isdigit`, `isalnum`, `isascii`, `isprint`
- Autres : `toupper`, `tolower`, `calloc`, `strdup`

### Partie 2 — Fonctions supplémentaires

- `substr`, `strjoin`, `strtrim`, `split`
- `itoa`, `strmapi`, `striteri`
- `putchar_fd`, `putstr_fd`, `putendl_fd`, `putnbr_fd`

---

## 🧪 Compilation & Utilisation

### Compilation

```bash
make
```

Pour nettoyer :

```bash
make clean      # Supprime les fichiers objets
make fclean     # Supprime les fichiers objets + libft.a
make re         # Recompile tout
```

### Utilisation dans un autre projet

Ajoutez `libft.a` à vos fichiers compilés :

```bash
gcc main.c -L. -lft
```

N'oubliez pas d'inclure le header :

```c
#include "libft.h"
```

---

## 🔎 Exemple d'utilisation

```c
#include "libft.h"
#include <stdio.h>

int main(void)
{
    char *str = "Hello World!";
    printf("Length: %zu\n", ft_strlen(str));
    return 0;
}
```

---
