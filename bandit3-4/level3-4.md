Bandit 3 → 4

We moved from the third level to the fourth level. The task for the new level is as follows:

Instruction:
The password for the next level is stored in a hidden file located in the inhere directory.

Useful commands:
ls, cd, cat, file, du, find

My solution:
First, I checked which directory I was in using the pwd command. Then I listed the contents of the directory with the ls command. Since ls did not show any files, I used the ls -la command to display hidden files as well. As mentioned in the instruction, I found a hidden file. The file name was:

...Hiding-From-You

To read the contents of the file, I used the cat command and enclosed the file name in quotation marks. As a result, I obtained the password:

cat "...Hiding-From-You"


Finally, I exited the third level by typing exit in order to proceed to the next stage.










Bandit 3 → 4

Üçüncü mərhələdən dördüncü mərhələyə keçid etdik. Yeni mərhələ üçün verilən tapşırıq aşağıdakıdır:

Təlimat:
Növbəti səviyyəyə aid parol inhere qovluğunda yerləşən gizli bir faylda saxlanılır.

Lazım ola biləcək əmrlər:
ls, cd, cat, file, du, find

Həll yolu:
Əvvəlcə hazırda hansı qovluqda olduğumu müəyyən etmək üçün pwd əmrindən istifadə etdim. Daha sonra ls əmri ilə qovluğun tərkibini yoxladım. ls əmri heç bir nəticə göstərmədiyi üçün gizli faylları da görmək məqsədilə ls -la əmrini icra etdim. Bu zaman təlimatda qeyd olunduğu kimi gizli bir fayl aşkar olundu. Faylın adı aşağıdakı kimi idi:

...Hiding-From-You

Faylın məzmununu oxumaq üçün cat əmrindən istifadə etdim və fayl adını dırnaq işarələri (“ ”) daxilində yazdım. Nəticədə parol əldə olundu:

cat "...Hiding-From-You"


Sonda yeni mərhələyə keçmək üçün exit əmrini yazaraq üçüncü səviyyədən çıxdım.
