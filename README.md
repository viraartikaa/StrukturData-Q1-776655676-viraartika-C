1. Kenapa Array $O(1)$ & Linked List $O(n)$?Array ($O(1)$): Memori kontinu (berdampingan). Komputer bisa langsung "lompat" ke alamat tujuan lewat perhitungan matematika sederhana karena jarak antar datanya pasti.Linked List ($O(n)$): Memori acak. Komputer harus menelusuri rantai dari awal satu per satu karena setiap data hanya tahu di mana lokasi data berikutnya.
Kapan Linked List Unggul?
Linked List lebih baik saat sering melakukan Penyisipan/Penghapusan di tengah atau awal data.

Alasan: Cukup ubah "tali" (pointer) antar node. Di Array, Anda harus menggeser semua elemen di belakangnya, yang memakan waktu lama jika datanya ribuan
Doubly Linked List
Struktur: Punya dua penunjuk: Next (ke depan) dan Prev (ke belakang).

Dampak: Memori lebih boros (butuh ruang untuk pointer tambahan), tapi navigasi jadi lebih fleksibel karena bisa mundur, tidak hanya maju.
Circular Linked List
Konsep: Ujung list (node terakhir) menyambung kembali ke Head (node pertama). Tidak ada null.

Contoh: Fitur "Repeat All" pada playlist musik atau sistem giliran pemain dalam game multiplayer.
Resizing pada Python List
Saat list penuh dan Anda melakukan append, Python melakukan:

Memesan "rumah baru" (memori) yang lebih besar.

Menyalin semua data lama ke rumah baru tersebut.

Membuang rumah lama.
Ini alasan mengapa sesekali append terasa sedikit lebih lambat dari biasanya.
