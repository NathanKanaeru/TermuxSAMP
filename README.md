![logo](large.png)

<p align="center">
    <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white">
</p>

# TermuxSAMP
**dengan tools ini , kamu dapat mengcompile script pawn kamu dengan menggunakan termux, gunakan sesuai kebutuhan. dapatlan versi original dari pawncompiler di [Official Github](https://github.com/pawn-lang/compiler)**

> [!NOTE]
> Projek ini sedang dalam masa pemgembangan

# TermuxSAMP

TermuxSAMP adalah proyek yang memungkinkan Anda untuk menggunakan Termux sebagai platform untuk mengembangkan dan menjalankan modifikasi SAMP (San Andreas Multiplayer) menggunakan compiler Pawn.

## Daftar Isi

- [Fitur](#fitur)
- [Persyaratan](#persyaratan)
- [Instalasi](#instalasi)
- [Penggunaan](#penggunaan)
- [Struktur Proyek](#struktur-proyek)
- [Kontribusi](#kontribusi)
- [Lisensi](#lisensi)

## Fitur

- Mendukung pengembangan modifikasi SAMP menggunakan Pawn compiler.
- Mudah digunakan di lingkungan Termux.
- Struktur proyek yang terorganisir.

## Persyaratan

- Termux (dapat diunduh dari [Google Play Store](https://play.google.com/store/apps/details?id=com.termux) atau [F-Droid](https://f-droid.org/packages/com.termux/)).
- Compiler Pawn.

## Instalasi

1. Clone repository ini ke Termux Anda:

    ```sh
    git clone https://github.com/username/TermuxSAMP.git
    cd TermuxSAMP
    ```

2. Instal compiler Pawn di Termux:

    ```sh
    pkg update
    pkg upgrade
    pkg install git make clang
    ```

## Penggunaan

1. Navigasi ke direktori proyek:

    ```sh
    cd TermuxSAMP
    ```

2. Mulai kompilasi file Pawn Anda:

    ```sh
    make
    ```

3. File hasil kompilasi akan disimpan di direktori `Release` atau `Debug`.

## Struktur Proyek

- **Application.mk**: File konfigurasi untuk build sistem.
- **CMAlloc.cpp, CMAlloc.h**: Modul untuk manajemen memori.
- **CMapRecorder.h**: Header untuk modul perekam peta.
- **DllMain.cpp**: Entry point untuk DLL.
- **IPatch.h**: Header untuk patching memori.
- **SAMP.cpp**: File sumber utama untuk SAMP.
- **CCheat.cpp, CCheat.h**: Modul untuk cheat.
- **CPatch.cpp, CPatch.h**: Modul untuk patching.
- **GTASA.h**: Header untuk integrasi dengan GTA San Andreas.
- **SAMP.h**: Header untuk SAMP.
- **IHook.h, IMAlloc.h, IMProt.h**: Header untuk hooking dan proteksi memori.
- **CHook.cpp, CHook.h**: Modul untuk hooking.
- **MemoryHackingFactory.cpp, MemoryHackingFactory.h**: Modul untuk manipulasi memori.
- **Debug/**: Direktori untuk build debug.
- **Release/**: Direktori untuk build release.

## Kontribusi

Kami menyambut kontribusi dari siapa saja. Jika Anda ingin berkontribusi, silakan fork repositori ini, buat branch baru, dan buat pull request. Harap pastikan kode Anda teruji dan mengikuti pedoman kontribusi.

## Lisensi

Proyek ini dilisensikan di bawah lisensi MIT. Lihat file [LICENSE](LICENSE) untuk informasi lebih lanjut.
