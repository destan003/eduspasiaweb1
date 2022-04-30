Sebelum upload ke netlify, kita coba bikin form dulu.

1. copy kan : name="contact" method="POST" data-netlify="true" ke form di halaman index kita

2. Copy kan juga : <input type="hidden" name="form-name" value="contact">
   taro di bawah tag form di halaman index.
3. Kita juga akan menambah filter spams nya. Copy : netlify-honeypot="bot-field"
   ke tag form di index.html nya

4. Copy pararaf: <p class="hidden">
<label>
Don’t fill this out if you’re human: <input name="bot-field" />
</label>
</p>

paste kan di bawah input hidden no 2 di atas.

5. Masuk ke style.css di atas navbar, bikin class hidden nya.
   .hidden {
   visibility: hidden;
   height: 0;
   }

6. Balik ke vs code untuk buka terminal.
7. Jika telah install Git untuk version manager, kita bikin repository nya di mesin. ketik : git init di folder directory nya.
8. akan terbentuk folder hidden .git
9. Masukan ke repo dsemuanya dengan ketik: git add .
