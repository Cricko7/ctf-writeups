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
1) Web
2) Network
3) Stegano
4) Crypto
5) OSINT
6) Reverse
7) Pwn
8) Forensics
9) Misc



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