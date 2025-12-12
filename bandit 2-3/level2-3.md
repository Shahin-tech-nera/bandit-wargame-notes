Bandit2 → Bandit3

We progressed from the second level to the third level. The instructions for the new level are as follows:

Instructions: The password for the next level is stored in the file named --spaces in this filename-- located in the home directory.

Useful commands: ls, cd, cat, file, du, find

bandit2@bandit:~$ ls
--spaces in this filename--
bandit2@bandit:~$ cat ./--spaces in this filename--
cat: ./--spaces: No such file or directory
cat: in: No such file or directory
cat: this: No such file or directory
cat: filename--: No such file or directory
bandit2@bandit:~$ cat -- ./--spaces in this filename--
cat: ./--spaces: No such file or directory
cat: in: No such file or directory
cat: this: No such file or directory
cat: filename--: No such file or directory
bandit2@bandit:~$ cat -- --spaces in this filename--
cat: --spaces: No such file or directory
cat: in: No such file or directory
cat: this: No such file or directory
cat: filename--: No such file or directory
bandit2@bandit:~$ cat -- "--spaces in this filename--"

As you can see, I first used the ls command to locate the file. Then I tried cat ./ and cat -- ./ to open it, but they didn’t work.

After doing some online research, I learned that cat treats filenames containing spaces or starting with -- as separate arguments.

The recommended solution is to use the -- option after the cat command. This tells the command that everything following -- is a filename, not an option.

Since our filename is --spaces in this filename-- and contains spaces, we can provide it in three ways:

Using double quotes: "..."

Using single quotes: '...'

Escaping spaces with \

Thus, the correct command to read the file is:

cat -- "--spaces in this filename--"

To proceed to the next level, we type exit to leave the second level.






Bandit2 → Bandit3

İkinci mərhələdən üçüncü mərhələyə keçdik. Yeni mərhələ üçün təlimat belədir:

Təlimat: Növbəti səviyyənin parolu ana qovluqda yerləşən --spaces in this filename-- adlı faylda saxlanılır.

Lazım ola biləcək əmrlər: ls, cd, cat, file, du, find

bandit2@bandit:~$ ls
--spaces in this filename--
bandit2@bandit:~$ cat ./--spaces in this filename--
cat: ./--spaces: No such file or directory
cat: in: No such file or directory
cat: this: No such file or directory
cat: filename--: No such file or directory
bandit2@bandit:~$ cat -- ./--spaces in this filename--
cat: ./--spaces: No such file or directory
cat: in: No such file or directory
cat: this: No such file or directory
cat: filename--: No such file or directory
bandit2@bandit:~$ cat -- --spaces in this filename--
cat: --spaces: No such file or directory
cat: in: No such file or directory
cat: this: No such file or directory
cat: filename--: No such file or directory
bandit2@bandit:~$ cat -- "--spaces in this filename--"

Gördüyünüz kimi, əvvəlcə ls əmri ilə faylı siyahıda tapdım. Daha sonra cat ./ və cat -- ./ ilə faylı açmağa çalışdım, amma alınmadı.

Bir az internet axtarışından sonra öyrəndim ki, cat əmri boşluqlar və -- ilə başlayan fayl adlarını ayrı-ayrı arqumentlər kimi qəbul edə bilər.

Buna görə tövsiyə olunur ki, cat əmrindən sonra -- işarəsi qoyulsun. Bu, komandaya bildirir ki, bundan sonra verilən arqumentlərin hamısı fayl adıdır, opsiya deyil.

Bizim fayl adı isə --spaces in this filename-- olduğu üçün, yəni boşluqlar ehtiva etdiyi üçün onu oxumağın üç yolu var:

Qoşa dırnaq "..." istifadə etmək

Tək dırnaq '...' istifadə etmək

Boşluqları \ ilə əvəz etmək

Beləliklə, faylı oxumaq üçün doğru əmr belədir:
cat -- "--spaces in this filename--"


