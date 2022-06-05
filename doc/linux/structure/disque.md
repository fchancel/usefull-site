# Disque

### # Definition

| Type         | Nom                                         | Description              |
| ------------ | ------------------------------------------- | ------------------------ |
| **sd**_xx_   | **S**olid **D**rive                         | Disque dure de type ssd  |
| **hd**_xx_   | **H**ard **D**rive                          | Disque dure de type hdd  |
| **nvme**_xx_ | **N**on-**V**olatile **M**emory **E**xpress | Disque dure de type nvme |

### # Definition de nomage pour

#### #ssd et #hdd

**\<type> \<register> \<partition>**

| Type | Register | Partition | Resulta |
| ---- | -------- | --------- | ------- |
| sd   | a        | 1         | sda1    |
| hd   | b        | 1         | hdb1    |

Le **Type** est le type de disque utilise

le **Register** definite l'ordre d'amorcage (**a** demarant en premieur par rapport au **b** ), commence de **a** et va jusqu'a **z**, si il ya plus de 26 (nombre de lettres dans l'alphabet) disque, on recomence avec 2 lettres **aa** ...

Le **Partition** est le numero de partition du disque, commence a **1**

#### # nvme

**\<type> \<register> N\<namespace> P\<partition>**

| Type | register | namespace | partition | Resulta   |
| ---- | -------- | --------- | --------- | --------- |
| nvme | 0        | n1        | p1        | nvme0n1p1 |

Le **Type** est le type de disque utilise

Le **register** definite l'ordre d'amorcage, commence a **0**

Le **namespace** definite le namespace des partitions, commence a **1**, preceder de la lettre **n**

Le **partition** est le numero de partition du disque, commence a **1**, preceder de la lettre **p**
