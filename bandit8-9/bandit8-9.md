Bandit8 → Bandit9

We progressed from the eighth level to the ninth level. The instructions for the new level are as follows:

Instructions: The password for the next level is stored in the file data.txt and is the only line of text that occurs exactly once.

Useful commands: grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

bandit8@bandit:~$ ls
data.txt
bandit8@bandit:~$ cat data.txt | tail -n 10
XVpgcRiZeeaxlFNA8MF1OA0yoQkU15Cr
H4dl3gUqaHje27iA3abJvJ6WS5EIYY2U
BMtzneXAcLAc3vynEF57mn1AdxECSqwF
JyFTMEaaGS62DoS6ZdkKrXPV8VuMaXXh
pvNw8dMAqtC0vrS9OjmgheVLXLFz9BUa
QYY6ADjYdtILCvm0QwTDHW5g4mGpPKur
rW1Tq5AEohYnVBImbJyX1cQ9IevwDg7Y
a8EPDYuGBd3mvar2s0aF5VFdaAY0GbUP
YGTz538EOOqQztF12JHBHXGPY7yY8jMp
8MNnqNdEQCk107HPCHvn10HhkUF607u4
bandit8@bandit:~$ sort data.txt | uniq -u
As you can see, I first used the ls command to check the file’s existence. Then I tried reading the file with cat, but it produced many long lines.

The task specifies that only the line that occurs exactly once is the correct password. After some research, I learned that using the sort command followed by uniq allows me to easily find this unique line.

Thus, the command to read the password for the next level is:

sort data.txt | uniq -u

Then we write exit and exit from 8th level. 








Bandit8 → Bandit9

Səkkizinci mərhələdən doqquzuncu mərhələyə keçdik. Yeni mərhələ üçün təlimat belədir:

Təlimat: Növbəti səviyyənin parolu data.txt faylında saxlanılır və yalnız bir dəfə rast gəlinən yeganə sətirdir.

Lazım ola biləcək əmrlər: grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

bandit8@bandit:~$ ls
data.txt
bandit8@bandit:~$ cat data.txt | tail -n 10
XVpgcRiZeeaxlFNA8MF1OA0yoQkU15Cr
H4dl3gUqaHje27iA3abJvJ6WS5EIYY2U
BMtzneXAcLAc3vynEF57mn1AdxECSqwF
JyFTMEaaGS62DoS6ZdkKrXPV8VuMaXXh
pvNw8dMAqtC0vrS9OjmgheVLXLFz9BUa
QYY6ADjYdtILCvm0QwTDHW5g4mGpPKur
rW1Tq5AEohYnVBImbJyX1cQ9IevwDg7Y
a8EPDYuGBd3mvar2s0aF5VFdaAY0GbUP
YGTz538EOOqQztF12JHBHXGPY7yY8jMp

Gördüyünüz kimi, əvvəlcə ls əmri ilə faylın mövcudluğunu yoxladım. Daha sonra cat əmri ilə faylı oxumağa çalışdım, amma çoxlu uzun sətirlər çıxdı.

Tapşırıqda isə yalnız təkrarlanmayan sətir düzgün parol kimi qəbul edilir. Bir az araşdırdıqdan sonra öyrəndim ki, bunu sort və uniq əmrləri ilə asanlıqla tapa bilərəm.

Beləliklə, növbəti səviyyənin parolunu tapmaq üçün istifadə ediləcək əmr:

sort data.txt | uniq -u

sonra exit yazib 8-ci leveldən çıxıriq.
