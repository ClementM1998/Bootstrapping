# Bootstrapping

`Persoalan saya:`
Apa kah saya boleh membuat bahasa pengaturcaraan sendiri yang kosong maksud saya kosong perpustakaan di buat dengan bahasa pengaturcaraan itu sendiri.

✅ 1. Reka sintaks asas
Mulakan dengan mencipta sintaks asas untuk:
* Perisytiharan pembolehubah
* Operasi aritmetik
* Kawalan aliran (if, while, for)
* Fungsi
* Struktur asas kelas (jika OOP)

`Contoh:`
```
int x = 10
print(x)
```

✅ 2. Bina compiler/interpreter asas
`Gunakan bahasa lain (contohnya C, C++, atau Java) untuk:`
* Parse kod anda (lexer + parser)
* Jalankan arahan (interpreter) atau hasilkan bytecode (compiler)

💡 Anda perlu bina:
* Tokenizer
* Parser
* AST builder
* Virtual Machine (jika interpreted)

✅ 3. Kosongkan semua fungsi perpustakaan
Pastikan bahasa anda:
* Tiada print, Math, String, System, dan sebagainya.
* Hanya menyokong operasi yang boleh dijalankan melalui instruction set yang anda buat.

`Contoh (kod peringkat rendah anda boleh jadi seperti):`
```
PUSH 10
PUSH 20
ADD
STORE x
```

✅ 4. Bina perpustakaan dalam bahasa itu sendiri
Sekarang, gunakan bahasa itu sendiri untuk membina semula fungsi asas seperti:
* print() → mungkin anda panggil fungsi VM secara dalaman
* Math.add() → anda tulis fungsi penambahan dalam bahasa itu
* String.length() → anda bina logik kiraan sendiri

