Membuat Portfolio menggunakan Tailwind
1. Membuat folder untuk menyimpa project
2. Buat file baru index.html
3. Buka Documentasi Tailwind, Installation CLI
4. Sebelum install tailwind, inisialisasi npm terlebih dahulu npm init -y
5. npm install -D tailwindcss
6. npx tailwindcss init
7. modifikasi config tailwind.config.js, pada content berikan 'index.html'
8. Add the Tailwind directives to your CSS, buat folder src sejajar dengan index.html, buat file input.css masukkan :
@tailwind base;
@tailwind components;
@tailwind utilities;
9. Start the Tailwind CLI build process
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch

-i sesuaikan dengan folder yang dibuat src dan file input.css
-o berada di folder yang sama, karena file output.css belum dibuat maka akan dibuatkan secara otomatis

CTRL + C, untuk keluar dari rebuild tailwind

10. Tambahkan extend > colors : {}, didalamnya jika sering menggunakan warna yang sama buatkan key primary: 'kode hex dari warna tsb'

