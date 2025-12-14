Bandit 9 → 10

We have progressed from the ninth level to the tenth level. The instructions for the new level are as follows:

Instruction:
The password for the next level is stored in the file data.txt. It is located in one of the few human-readable strings and is preceded by several = characters.

Commands that may be useful:
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

My Solution

When executing the command cat data.txt, a long sequence of unreadable characters and symbols is displayed. Upon careful inspection, it is possible to notice that, as stated in the level instructions, the password appears in plain text preceded by several = characters.

However, manually searching through this disordered output is inefficient. Therefore, the appropriate approach is to extract only the human-readable strings from the file. This can be achieved using the strings command. To further narrow down the results and identify the line containing the password, the output is filtered using the grep command:

strings data.txt | grep "="

As a result, the line containing the password is revealed.

To proceed to the next level, I exit level 9 by entering the exit command.










Bandit 9 → 10

Doqquzuncu mərhələdən onuncu mərhələyə keçdik. Yeni mərhələ üçün verilən təlimat aşağıdakı kimidir:

Təlimat:
Növbəti səviyyə üçün parol data.txt faylında saxlanılır. Parol insan tərəfindən oxuna bilən bir neçə sətirdən birində yerləşir və ondan əvvəl bir neçə = simvolu mövcuddur.

Lazım ola biləcək əmrlər:
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

Mənim həllim

cat data.txt əmrini icra etdikdə, ekranda uzun və anlaşılmaz simvollar toplusu əks olunur. Diqqətlə baxdıqda, mərhələnin şərtində qeyd edildiyi kimi, mətnin daxilində bir neçə = işarəsindən sonra parolun açıq şəkildə göründüyünü müşahidə etmək mümkündür.

Lakin bu cür qarışıq məlumat arasında əl ilə axtarış aparmaq səmərəli olmadığı üçün, faylın daxilində insan tərəfindən oxuna bilən sətirləri çıxarmaq məqsədəuyğundur. Bunun üçün strings əmrindən istifadə edirik. Daha sonra isə = simvolunu ehtiva edən sətirləri filtrdən keçirmək üçün grep əmrindən yararlanırıq:

strings data.txt | grep "="

Bu əmrin nəticəsində parol olan sətir aşkar edilir.

Yeni mərhələyə keçmək üçün exit əmrini yazaraq doqquzuncu səviyyədən çıxış edirəm.
