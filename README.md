# ctf-writeups

> Изменено 24.02.2026

# Мой опыт в CTF-соревнованиях / ctf-writeups

### О себе

- ФИО:
> Степанов Роман Сергеевич

- Возраст:
> 22

- Образование:
> Получаю ВО (есть диплом СПО). Есть квалификация "техник по защите информации".

- Страна:
> Россия

- Город:
> Ростов-на-Дону

### Опыт:
- Количество соревнований: 2
- - Количество командных: 1
- - Количество одиночных: 1

Категорий заданий (по приоритету):
<p align="center">
  [![Web #1](https://img.shields.io/badge/web-🔥%231-brightgreen?style=flat-square&logo=firefox&logoColor=white)](./web/)
  [![Network #2](https://img.shields.io/badge/network-⚡%232-blue?style=flat-square&logo=network&logoColor=white)](./network/)
  [![Stegano #3](https://img.shields.io/badge/stego-🖼️%233-teal?style=flat-square&logo=image&logoColor=white)](./stego/)
  [![Crypto #4](https://img.shields.io/badge/crypto-🔐%234-blue?style=flat-square&logo=sagemath&logoColor=white)](./crypto/)
  [![OSINT #5](https://img.shields.io/badge/osint-🔍%235-orange?style=flat-square&logo=detective&logoColor=white)](./osint/)
  [![Reverse #6](https://img.shields.io/badge/re-🔄%236-yellow?style=flat-square&logo=rust&logoColor=black)](./reverse/)
  [![Pwn #7](https://img.shields.io/badge/pwn-💥%237-red?style=flat-square&logo=python&logoColor=white)](./pwn/)
  [![Forensics #8](https://img.shields.io/badge/forensics-🔎%238-purple?style=flat-square&logo=wireshark&logoColor=white)](./forensics/)
  [![Misc #9](https://img.shields.io/badge/misc-🎲%239-gray?style=flat-square&logo=dice&logoColor=white)](./misc/)
</p>




## Древо:

```
cricko7/ctf-writeups/
│
│
├── README.md    # Главная страница
|
|
├── .gitignore   # Игнор временных файлов, *.pyc, .DS_Store
│
|
|
├── crypto/       # Криптография
│   │
│   ├── anyctf-2026/           # Название CTF + год
│   │   └── easy-rsa/
│   │       ├── README.md     # Описание задачи, очки, solves
│   │       ├── solve.py      # Ваш скрипт решения
│   │       ├── challenge/    # Исходники задач
│   │       │   └── rsa_easy.enc
│   │       └── images/       # Скриншоты, диаграммы
│   │           └── factor_attack.png
│   │
│   └── anyctf-2026/
│       └── quantum-break/
│           ├── README.md
│           └── solve.rs   # Rust-скрипт для атаки
│
├── pwn/                # Binary exploitation
│   └── anyctf-2026/
│       └── baby-heap/
│           ├── README.md
│           ├── exploit.py
│           ├── challenge/
│           │   └── baby_heap
│           └── images/
│               └── gdb_session.png
│
├── web/           # Web exploitation
│   └── anyctf-2026/
│       └── ssti-injection/
│           ├── README.md
│           ├── exploit.js
│           └── challenge/
│               └── app.py
│
├── reverse/       # Reverse engineering
│   └── anyctf-2026/
│           └── any_crackme-v2/
│               ├── README.md
│               ├── solve.py
│               └── challenge/
│                   └── crackme_v2.bin
│
├── forensics/     # Forensics
│   └── anyctf-2026/
│       └── memory-leak/
│           ├── README.md
│           ├── volatility_profile
│           └── images/
│               └── any_strings_output.png
│
├── misc/   # Разное (stego, hardware и т.д.)
│
│
│
│
│
│
└── tools/    # Утилиты
    │
    │
    ├── crypto-tools/
    │   
    └── pwn-tools/
        

```

#### Таблица:

| Категория | Основные инструменты           | Альтернативы                      | Docker образы                        |
| --------- | ------------------------------ | --------------------------------- | ------------------------------------ |
| Crypto    | Sage, RsaCtfTool, factordb.com | yafu, msieve, cryptool            | docker run -it cryptool/ctf-crypto   |
| Pwn       | pwntools, ROPgadget, checksec  | gef, PEDA, one_gadget             | docker run -it pwn/ctf-pwn           |
| Reverse   | Ghidra, radare2, Cutter        | IDA Free, Binary Ninja, retdec    | docker run -it ghidra/ctf-re         |
| Web       | Burp Suite, sqlmap, nuclei     | ffuf, dirsearch, wpscan           | docker run -it burpsuite/ctf-web     |
| Forensics | Wireshark, binwalk, volatility | foremost, scalpel, autopsy        | docker run -it sundeeparya/ctf-tools |
| Stego     | Stegsolve, zsteg, steghide     | outguess, stegseek, stegonline    | docker run -it stego/ctf-stego       |
| Misc      | CyberChef, hashcat, nc         | base64decode.org, man-db, xxd     | docker run -it cyberchef/ctf-misc    |
| Network   | Wireshark, tcpdump, nmap       | netcat, wireshark-tshark, masscan | docker run -it nmap/ctf-network      |
| Android   | Frida, jadx, apktool           | objection, mobSF, drozer          | docker run -it frida/ctf-android     |