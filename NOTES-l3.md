
## 1. stash list
```text
stash@{0}: On lab3/variant-5-vyshnevskyi: чернетка ліцензії v5
```
## 2. cherry-pick
```text
feature/pick-5: cf3c45b
lab3/variant-5-vyshnevskyi: 6bbe211
```.

## 3. reflog
```text
803efd9 (HEAD -> lab3/variant-5-vyshnevskyi) HEAD@{0}: commit (amend): Зафіксувати ліцензію, варіант 5
6bbe211 HEAD@{1}: cherry-pick: Уточнити ліцензію
a951fee HEAD@{2}: checkout: moving from feature/pick-5 to lab3/variant-5-vyshnevskyi
cf3c45b (feature/pick-5) HEAD@{3}: commit: Уточнити ліцензію
a951fee HEAD@{4}: checkout: moving from lab3/variant-5-vyshnevskyi to feature/pick-5
```
## 4. revert
```text
22026f3 (HEAD -> lab3/variant-5-vyshnevskyi, origin/lab3/variant-5-vyshnevskyi) Revert "Зіпсувати рядок"
5b1dee5 Зіпсувати рядок
```
## 5. тег
```text
22026f3 (HEAD -> lab3/variant-5-vyshnevskyi, origin/lab3/variant-5-vyshnevskyi) Revert "Зіпсувати рядок"
5b1dee5 Зіпсувати рядок
803efd9 Зафіксувати ліцензію, варіант 5
a951fee Зберегти відновлену чернетку v5
d8de6a0 Створити файл варіанта 5
5c11f1f (origin/main, origin/HEAD, main) Initial commit

 tag: v0.1-vyshnevskyi, origin/lab3/variant-5-vyshnevskyi)
Author: nvishurl <nvishurl@gmail.com>
Date:   Thu Nov 12 05:54:48 2026 +0200

    Revert "Зіпсувати рядок"

    This reverts commit 5b1dee54727b9c4e124b1159e14a8d751446a1e6.
```
## 6. rebase -i
```text
pick [ХЕШ] WIP: чернетка
squash [ХЕШ] fix typo
Підсумкове повідомлення: Уточнити ліцензію
```
## 7. blame
```text
d8de6a0 (nvishurl 2026-11-12 05:48:05 +0200 1) # Ліцензія — варіант 5
```

## 8. fork
origin мій власний репозиторій на GitHub.
upstream оригінальний репозиторій, із якого створено fork.
Зміни з upstream отримують через git fetch upstream.
Свої коміти відправляють через git push origin, а PR створюють до upstream/main.

Посилання на репозиторій: https://github.com/nvishurl/git-lab-3
Посилання на гілку: https://github.com/nvishurl/git-lab-3/tree/lab3/variant-5-vyshnevskyi
Посилання на тег: https://github.com/nvishurl/git-lab-3/releases/tag/v0.1-vyshnevskyi
