Bandit7
When I reached Bandit7, I had already completed the challenges of the sixth level. Now a new task stood before me. According to the instructions, the password for the next level was hidden inside a file called data.txt, right next to the word “millionth.” A list of potentially useful commands was also provided: man, grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd.

First, I returned to my terminal and connected to the Bandit7 level with:
ssh bandit7@bandit.labs.overthewire.org -p 2220

The system prompted me for a password, so I carefully pasted the one I had recovered in the previous level. After a brief moment, a welcome message appeared, confirming that I had successfully entered Bandit7.

My first step was to check the directory contents using ls. As expected, there was a large file named data.txt. I knew it contained millions of lines, so manually checking it was impossible.

Instead, I went straight for the target. I typed the following command:
cat data.txt | grep millionth

After a quick search, the password appeared on the screen—the key to the next level! Knowing I had completed the task, I felt a sense of relief.

The final step was simple: I typed exit to leave the level and prepared to move on to the next challenge.





Bandit7
Bandit7 səviyyəsinə keçəndə artıq altıncı mərhələnin sınaqlarını uğurla arxada qoymuşdum. Qarşımda yeni bir tapşırıq dururdu. Təlimata əsasən, növbəti səviyyənin parolu data.txt adlı faylda, “millionth” — yəni “milyonuncu” sözünün yanında gizlədilmişdi. Bu mərhələdə mənə lazımlı ola biləcək əmrlərin siyahısı da verilmişdi: man, grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd.

Əvvəlcə terminala qayıdıb aşağıdakı əmrlə Bandit7 səviyyəsinə daxil oldum:
ssh bandit7@bandit.labs.overthewire.org -p 2220

Sistem məndən parol istədi. Mən isə əvvəlki — altıncı mərhələdən tapdığım parolu diqqətlə kopyalayıb yapışdırdım. Bir neçə saniyə sonra ekranda tanış salamlaşma mesajı göründü və bununla da Bandit7 səviyyəsinə daxil olduğumu anladım.

İlk işim ls əmri ilə direktoriyada hansı faylların olduğunu yoxlamaq oldu. Gözlədiyim kimi, data.txt adlı böyük bir fayl orada idi. Faylın içində milyonlarla sətir olduğunu bilirdim, ona görə əlinə baxmaq mümkün deyildi.

Mən isə birbaşa hədəfə yönəldim. Terminalda aşağıdakı əmri yazdım:
cat data.txt | grep millionth

Bir anlıq axtarışdan sonra ekranda parol peyda oldu — məhz növbəti səviyyəyə açarı verən o söz! Tapşırığı tamamladığımı bilərək rahat nəfəs aldım.

Sonuncu addım isə sadə idi: exit yazıb bu səviyyədən çıxdım və növbəti mərhələyə doğru addımladım.
