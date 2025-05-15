---
date: 2025-05-15T19:20:32+07:00
draft: false
title: AI (gak) selalu bisa diandalkan 
hideReadingTime: true
hideWordCount: true
---

Halo ⸜(｡˃ ᵕ ˂ )⸝♡

Kayannya udah hampir dua minggu lebih ga ngeblog :v

Lagi fokus sama project soalnya ;"

Karena udah mau selesai,nulis dikit ah~

Ah, AI siapa sih yang ga kenal mereka sekarang ini? Mulai dari chatbot sampe tools pembuat gambar,seengaknya kita pasti pernah make salah satu dari mereka (kecuali kalo kalian itu gaptek ._.)

Udah kaya alat serba bisa dimana kita bisa bikin gambar atau nyari informasi dengan lebih mudah² pake kuadrat karena sebelum ada AI dua hal itu emang udah mudah bahkan sebelum ada AI(kecuali bikin gambar sih hehe).

Ya karena kemudahannya banyak orang yang make termasuk para programmer malas(kaya aku :V).  
*Note: Aku gak asal copas dan cuma nyuruh AI kalau ada tugas repitif kaya nulis banyak HTML(malazzz) atau emang mager aja buka google atau ga error ga jelas yang ga bisa dicari pencaariang google.*

Jadi ya,hasilnya apa? ngerjain project jadi lebih cepat lah :v

Yang awalnya seminggu bisa jadi 3 hari dan itu udah termasuk waktu leha leha hehehe.

Tetapi....ga ada hal yang sempurna :(

Jadi gini,aku ada project bikin sistem CRUD(create read update delete), disitu aku make tools namanya prisma untuk mempermudah manage data di database.

Programmer rajin pasti bakal baca dokumentasi(panduan) dari sebuah tools sebelum dipake.Tapi kan aku pemalas =w=

Ya jadi akupun nanya chatgpt gimana cara make prisma.

Dan langsung dikasih panduannya.  

Ringkas,padat,to the point ga pake ba bi bu kaya dokumentasi resmi nya.

Lalu dimana masalahnya?

Nah jadi chatgptp ngasih aku beberapa command untuk menggunakannya:

```bash
npm install prisma

npx prisma init

npx prisma generate

npx prisma mirgate dev
```

Gausah dijelasin line by linenya dah,malas :v

Nah setelah semuanya command nya dijalankan, aku pengen make prisma di dalam script yang udah ada,menurut chat gpt caranya begini:

```javascript
const { PrismaClient } = require("@prisma/client");
```

Hasilnya? Malah dong TwT.

Aku pun bolak balik nanya chat gpt, solusinya(menurut dia) dengan jalanin command `npx prisma generate`.

Tapi tetep ga berhasil.

Setelah terus menerus tanya aku pun mau ga mau ya harus baca dokumentasi,dan bener aja disana ada jawabannya.

Bangke...

Menurut dokumentasi prisma kode import yang benar adalah:
```javascript
const { PrismaClient } = require("./generated/prisma");
```

Ya itu aja :|

Aku harusnya import library yang digenerate sama prisma,bukan import library yang keinstall.

5 jam+ habis untuk benerin error ternyata cuma salah import doang.

Capek dehhhh....

Dan itulah mending jangan terlalu bergantung sama AI(kecuali bikin HTML hehehe).