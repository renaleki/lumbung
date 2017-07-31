## Sinkronisasi Upstream
Metode fork mengharuskan kita untuk selalu melakukan sinkronisasi dengan upstream / repositori induk [bgli/lumbung](https://github.com/bgli/lumbung).
Pada laman ini akan dijelaskan bagaimana mengatur repositori lokal agar tetap selaras dengan repositori induk.

## 1. Tambahkan Alamat Git Remote
```
git remote add upstream git@github.com:bgli/lumbung.git
```

## 2. Lakukan Pull / Tarik dari Upstream
```
git pull upstream master
```
Sehingga akan muncul commit message editor 

```
Merge branch 'master' of github.com:bgli/lumbung

# Please enter a commit message to explain why this merge is necessary,
# especially if it merges an updated upstream into a topic branch.
#
# Lines starting with '#' will be ignored, and an empty message aborts
# the commit.
~
~
~
...
```

Ketik `:q` untuk keluar dari commit message editor

Jika berhasil akan muncul pesan seperti contoh di bawah ini

```
remote: Counting objects: 14, done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 14 (delta 3), reused 13 (delta 2), pack-reused 0
Unpacking objects: 100% (14/14), done.
From github.com:bgli/lumbung
 * branch            master     -> FETCH_HEAD
 * [new branch]      master     -> upstream/master
Merge made by the 'recursive' strategy.
 README.md | 24 +++++++++++++++++++++++-
 1 file changed, 23 insertions(+), 1 deletion(-)
 ```
