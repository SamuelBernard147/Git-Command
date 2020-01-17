# Git_Command
Catatan personal dalam penggunaan git sehari hari
TODO :
- Rapihin markdown

// Inisialisasi
git init

// Nambah url
git remote add origin (copas url git)
git remote -v

// Add file
git add .
git commit -m "nama commit"

// Upload lokal -> remote
git push -u origin master

// ngambil revisi
git fetch -u origin master (ketahan)
git pull -u origin master (langsung)

// pindah branch
git checkout master

//gabungin remote -> lokal
git merge origin/master (remote -> lokal)

//download 
git clone (url)

//riwayat
git log --oneline

//perubahan
git diff 

// Update project hasil fork
# Tambah repositori asal, dinamain "upstream":
git remote add upstream https://github.com/whoever/whatever.git

# Ngambil semua update dari repositori asal,
# contoh upstream/master:
git fetch upstream

# pastiin lagi di branch master repositori lokal:
git checkout master

# Nulis ulang branch master jadi histori commit yang gk ada di upstream/master jadi ada di branch local lain :
git rebase upstream/master
