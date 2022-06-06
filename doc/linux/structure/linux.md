# linux

information from linux

### # Hiarchy

| Chemin       | Nom                                     | Description                                                                                                               |
| ------------ | --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| /bin         | **Bin**ary                              | Contient les commandes Unix essentielles                                                                                  |
| /usr/bin     | ""                                      | idem que _/bin_ mais pour utilisateur                                                                                     |
| /usr/sbin    | **S**uper-utilisateur **Bin**ary        | Commandes utilisees par le super-utilisateur                                                                              |
| /usr/lib     | **Lib**rary                             | Bibliotheques standard                                                                                                    |
| /usr/lib/X11 | **X**-windows version **11**            | Bibliotheque de x11                                                                                                       |
| /usr/include | --                                      | Repertoire standard des fichier heard en language c                                                                       |
| /usr/src     | **S**ou**rc**e                          | Fichier sources du systeme                                                                                                |
| /usr/local   | --                                      | Contient les programmes ajouter localement parle super-utilisateur                                                        |
| /sbin        | **S**ysteme **Bin**ary                  | Contient les commandes necessaires pour le systeme , est charger avant /usr                                               |
| /boot        | --                                      | Le noyaux et certains fichier necessaires a l'amorcage du systeme                                                         |
| /etc         | **E**ditable **T**ext **C**onfiguration | Fichier de configuration du systeme et applications                                                                       |
| /etc/skel    | ??                                      | Contient les models de fichier de configuration et de demarrage qui sont copie a **/home** pour tout nouvelle utilisateur |
| /dev         | **Dev**ices                             | Contient les interfaces entre le systeme et les peripheriques                                                             |
| /proc        | **Proc**esor                            | Contient les interfaces entre le systeme et le processeur, processurs actifs et la memoires                               |
| /var         | --                                      | Fichier de trace(log) du systeme                                                                                          |
| /home        | --                                      | Contient tout les dossiers des utilisateur                                                                                |
| /tmp         | **Tem**poary                            | Dossier de stokage de fichier temporaire, ce vide a tout demarage systeme                                                 |
| /mnt         | **M**ou**nt**                           | Dossier ou ce trouve les disques dure externe monte                                                                       |
| /sys         | **sys**teme                             | Dossier ou ce trouve les fichiers du systeme                                                                              |
| /srv         | ??                                      | ??                                                                                                                        |
| /opt         | **Opt**ion                              | Resemble a **/usr/local** mais pour les utilisateurs classic                                                              |

#### # Fichiers

| Chemin                 | Type    | Description                                               |
| ---------------------- | ------- | --------------------------------------------------------- |
| /boot/**vmlinuz-XXXX** | Binaire | Kernel linux                                              |
| /etc/fstab             | Text    | List les systemes de fichiers a montee au demarage        |
| /etc/passwd            | Text    | Liste les utilisateurs du systeme                         |
| /etc/shadow            | Text    | Liste les mots de passe (chiffre) utilisateurs du systeme |

#### # Glossaires

| Type          | Nom                                       | Desceription                                                                      |
| ------------- | ----------------------------------------- | --------------------------------------------------------------------------------- |
| fichier \*.rc | **R**essource **C**onfiguration           | Fichier de configuration                                                          |
| LVM           | **L**ogical **V**olumes **M**anager       |                                                                                   |
| MBR           | **M**aster **B**oot **R**ecord            | Secteur d'amorcage du systeme qui permet de demarrer de systeme voire _partition_ |
| GRUB          | **GR**and **U**nified **B**oot loader     | Chargeur de systeme qui cherche les **MBR**                                       |
| LILO          | **Li**nux **Lo**ader                      | Chargeur de systeme, a ete remplacer par **GRUB**                                 |
| SWAP          | --                                        | Fichier de memoire virtuelle utiliser par linux pour de l'optimisation            |
| TTY           |
| DMA           | **D**irect **M**emory **A**cess           | Cannaux d'acces direct a la memoire                                               |
| FHS           | **F**ilesystem **H**ierarchy **S**tandard | Convention standard de lahiarchy du systeme linux                                 |
