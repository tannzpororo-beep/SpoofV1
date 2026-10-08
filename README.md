# TannnSpoof

TannnSpoof adalah PWA + Roblox Studio plugin untuk:
- menyimpan banyak Animation ID;
- membuat mapping ID lama → ID baru;
- mengekspor mapping Luau;
- preview Animation ID secara nyata pada rig di Roblox Studio.

## Penting
Roblox tidak menyediakan mekanisme resmi untuk membuat "ID animasi palsu" yang berlaku online. Animation ID yang dapat dipakai dalam game harus merujuk ke asset yang tersedia/diizinkan oleh Roblox.

Plugin ini sengaja tidak melakukan bypass permission, moderation, atau ownership.

## Instalasi
1. Buka `TannnSpoof.html` di browser atau host sebagai static PWA.
2. Untuk preview nyata, pasang `studio-plugin/TannnSpoof.plugin.lua` sebagai plugin Roblox Studio.
3. Di Studio pilih rig yang memiliki Humanoid/AnimationController + Animator.
4. Buka TannnSpoof dari toolbar, masukkan Animation ID, lalu Preview.

## Publishing tanpa klik manual?
Untuk upload animation, Roblox saat ini menyediakan workflow resmi melalui Studio/Creator Dashboard. Open Cloud Assets API juga mendukung upload asset Animation dalam format `.rbxm`/`.rbxmx`, tetapi membutuhkan API key/OAuth dengan permission yang sesuai. Jangan menaruh API key di PWA client-side; gunakan backend/server-side proxy jika nanti fitur upload cloud ditambahkan.
