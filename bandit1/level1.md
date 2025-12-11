Bandit1
After successfully completing Level 0, I moved on toward Level 1. A new instruction appeared on the screen: the password for the next level is stored in a file named “-” located in the home directory.
The useful commands listed were: ls, cd, cat, file, du, find.

To access the first level, I typed:
ssh bandit1@bandit.labs.overthewire.org -p 2220

The system asked for a password. I copied the password I had retrieved from Level 0 and pasted it. A moment later, the Bandit1 environment opened, showing a short welcome message.

I reminded myself of an important habit:
“Starting from Level 0, I should store every password I find in a dedicated folder. Inside that folder, I’ll use an Excel file to keep everything organized — one column for the level number, and one for the password. No need for a Word document; Excel is much cleaner for this.”

Then I ran the ls command. Only a single dash “-” appeared. At first sight it seemed meaningless. But running ls -la revealed that it was actually a file.

I initially thought I could simply run cat - to open it. But that didn’t work — Linux treated the dash not as a file name, but as input (stdin). So the file wasn’t opened.

The solution was to explicitly tell Linux that the file is located in the current directory.
First, I checked my location using pwd, and navigated if needed using cd.

Once I confirmed I was in the correct directory, I executed:
cat ./-

This time, Linux recognized “-” as the name of the file in the current directory and displayed its contents. The password for the next level finally appeared.

I immediately copied the password into my Excel file so it wouldn’t get lost.

After finishing everything, I typed exit to leave Level 1.

One final note I almost forgot to mention:
“After finding the password in Level 0, you must exit that session before connecting to Level 1.”




Bandit1
Sıfırıncı mərhələni uğurla keçib birinci mərhələyə doğru yola düşdüm. İndi qarşıma yeni təlimat çıxırdı: növbəti səviyyənin parolu home directory-də yerləşən “-” adlı faylda saxlanılırmış.
Tövsiyə olunan əmrlər isə bunlardır: ls, cd, cat, file, du, find.

Birinci mərhələyə keçmək üçün terminalda belə yazdım:
ssh bandit1@bandit.labs.overthewire.org -p 2220

Məndən parol tələb olundu. Sıfırıncı mərhələdə tapdığım parolu copy‑paste etdim və beləliklə Bandit1 səviyyəsinə daxil oldum. Terminalda qısa bir salamlama mətninin çıxdığını gördüm.

Daxilimdə bir qeyd də etdim:
“Sıfırıncı mərhələdən başlayaraq tapdığım bütün parollar üçün ayrıca bir qovluq yaratmalıyam. O qovluqda bir Excel faylı açıb hər səviyyənin nömrəsini və parolunu ayrıca xanaya yazsam, sonradan heç nə it‑bat olmayacaq.”
Word sənədi ilə vaxt itirməyə ehtiyac yox idi — Excel bunun üçün ideal idi.

Sonra ls əmrini verdim. Nəticə olaraq təkcə bir tire işarəsi “-” çıxdı. İlk baxışda çox mənasız görünürdü. Lakin ls -la yazanda bunun əslində fayl olduğunu anlamaq olurdu.

Əvvəlcə düşündüm ki, sadəcə cat - yazıb faylı açaram. Amma təcrübə göstərdi ki, bu belə işləmir: Linux bunu fayl adı deyil, əmrdən sonra verilən giriş (stdin) kimi qəbul edir. Yəni fayl oxunmurdu.

Həlli isə sadə idi: tire ilə başlayan faylları oxumaq üçün onların cari qovluqda olduğunu göstərmək lazımdır. Bunun üçün əvvəlcə pwd ilə hansı qovluqda olduğumu yoxladım. Lazım olarsa cd ilə düz qovluğa keçməli idim.

Nəhayət, düzgün yerdə olduğuma əmin olandan sonra əmri yazdım:
cat ./-

Bu dəfə Linux tire işarəsinin əslində cari qovluqdakı fayl adı olduğunu anladı və faylın içini göstərdi. Beləcə, növbəti mərhələnin parolu ekranda göründü.

Parolu dərhal Excel cədvəlimə köçürdüm ki, itməsin.

İşimi bitirib exit yazaraq Bandit1 səviyyəsindən çıxdım.

Sonda bir vacib qeydi də əlavə etməliyəm:
“Sıfırıncı mərhələdə parolu tapdıqdan sonra birinci mərhələyə keçmək üçün mütləq sıfırıncı mərhələdən çıxmaq lazımdır. Bunu əvvəl deməyi unutmuşdum.”
