# Bandit0

To begin the game, I open the link provided in the Introduction section, and I am greeted with Level 0. Here, I can see the instructions and the exact command needed to connect. Since it is my first time entering the game, I use the SSH command shown on the page:

ssh bandit0@bandit.labs.overthewire.org -p 2220


When I asked what this command means, it was explained as follows:  
`ssh` stands for **Secure Shell**, which is used to securely connect to a remote machine or server.  
`bandit0` refers to the username for Level 0 of the game.

**Note:** ChatGPT informed me that OverTheWire’s security policy prohibits sharing passwords publicly. This is important to follow to remain within the rules.

The hostname `bandit.labs.overthewire.org` was taken directly from the official website.  
The `-p` option followed by `2220` specifies the special port number that must be used to connect.

---

## Instructions for Moving from Level 0 to Level 1

The website provides the following instruction:

> “The password for the next level is stored in a file named **readme** located in the home directory. Use this password to log into **bandit1** via SSH. Whenever you find a password, use SSH (on port 2220) to move to the next level and continue the game.”

It also lists the commands that may be helpful for solving the level:  
`ls`, `cd`, `cat`, `file`, `du`, `find`

---

## My Solution

After connecting to the server through SSH, a welcome message appears, and the terminal becomes ready for input. Then I proceed as follows:

1. I run the `ls` command, which reveals a file named **readme** in the directory.
2. I execute `cat readme` to read the contents of the file. This displays the password for the next level.

However, **in compliance with OverTheWire rules and security guidelines, I do not share the password here**.

---










# Bandit0

Oyuna başlamaq üçün Introduction bölməsində qeyd etdiyim linkə daxil oluram və məni sıfırıncı səviyyə qarşılayır. Burada qoşulmaq üçün təlimatlar və istifadə etməli olduğum kod göstərilir. Oyuna ilk dəfə daxil olduğum üçün proses mənə tam aydın deyildi, buna görə ChatGPT-dən kömək istədim. O, mənə terminalda aşağıdakı əmri daxil etməyi öyrətdi:

ssh bandit0@bandit.labs.overthewire.org -p 2220


Bu əmrin nə demək olduğunu soruşduqda belə izah olundu: `ssh` — *secure shell*, yəni uzaqdakı bir kompüterə və ya serverə təhlükəsiz şəkildə qoşulmaq üçün istifadə olunur. `bandit0` isə oyunda sıfırıncı səviyyəyə daxil olduğumu bildirir. Bu səviyyənin parolu əvvəlcədən təqdim olunur.

**Qeyd:** ChatGPT mənə OverTheWire platformasının təhlükəsizlik siyasətinə görə parolları açıq şəkildə paylaşmamağı tövsiyə etdi. Bu, qaydalara uyğun davranmaq üçün vacibdir.

`bandit.labs.overthewire.org` ünvanını ChatGPT saytın özündən götürüb. `-p` parametrinin qarşısında yazılan `2220` isə bizim qoşulmağımız üçün açıq qoyulan xüsusi port nömrəsidir.

---

## Sıfırıncı mərhələdən birinci mərhələyə keçid üçün təlimat

Saytda verilən təlimat belədir:

> “Növbəti səviyyə üçün parol ana qovluqda yerləşən **readme** adlı faylda saxlanılır. Bu paroldan istifadə edərək SSH vasitəsilə **bandit1** səviyyəsinə daxil olun. Hər dəfə parolu tapdıqda həmin səviyyəyə qoşulmaq üçün yenidən SSH (port 2220) istifadə edin.”

Bu mərhələdə istifadə edə biləcəyimiz əmr siyahısı da verilir:  
`ls`, `cd`, `cat`, `file`, `du`, `find`

---

## Mənim həll yolum

SSH vasitəsilə serverə qoşulduqdan sonra ekranda qısa bir salamlama mesajı çıxır və terminal əmrləri üçün hazır vəziyyətdə oluram. Ardınca:

1. `ls` əmrini daxil edirəm. Nəticədə qovluqda **readme** adlı faylın olduğunu görürəm.  
2. `cat readme` yazıb faylın içini oxuyuram. Nəticədə növbəti səviyyənin parolu ekranda görünür.

Lakin yenə də **təhlükəsizlik və OverTheWire qaydalarına uyğun olaraq parolu burada paylaşmıram**.

---
