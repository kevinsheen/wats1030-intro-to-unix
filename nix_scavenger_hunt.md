# *nix Scavenger Hunt

Complete the following challenges using the command-line interface on your favorite
Unix or Linux operating system. You are welcome and encouraged to consult any
additional documentation online or in books.

Please add your answers/responses/text pastes to the document after each prompt.

Note: For some of the challenges you will need to reference files included with
this repository, so you will need to fork the repo into your own Github account
and then clone it to your development environment.

## The Challenges

### Navigating the Filesystem

* Get an idea of where you are in the operating system. Use the `pwd` command to find your "path to working directory"--your current location in the filesystem of your devbox. *Paste the output of the `pwd` command here:* /home/cabox/workspace

* Discover more about this filesystem. Use `ls` (the "list" command)to see what is in this directory. *What directories and files do you see when you run `ls`?* LICENSE    challenge_files        nix_scavenger_hunt_stretch.md         
README.md  nix_scavenger_hunt.md 

* You can use *options* to modify how a command runs. Try using `ls -alh` to see the contents of your current directory. *How are the results different when you use the `-alh` options?* total 36K                                                               
drwxrwxr-x  4 cabox cabox 4.0K Apr  9 00:52 .                           
drwxr-xr-x 11 cabox cabox 4.0K Apr  9 00:52 ..                          
drwxrwxr-x  8 cabox cabox 4.0K Apr  9 00:52 .git                        
-rw-rw-r--  1 cabox cabox 1.1K Apr  9 00:52 LICENSE                     
-rw-rw-r--  1 cabox cabox 1.4K Apr  9 00:52 README.md                   
drwxrwxr-x  7 cabox cabox 4.0K Apr  9 00:52 challenge_files             
-rw-rw-r--  1 cabox cabox 5.6K Apr  9 15:39 nix_scavenger_hunt.md       
-rw-rw-r--  1 cabox cabox  317 Apr  9 00:52 nix_scavenger_hunt_stretch.md  

* The `man` ("manual") command tells you more about how any given command works. (*WARNING:* CodeAnywhere does not support the man command. You can click the following link to complete this task: http://linux.die.net/man/)Run `man` to see instructions about how to use `man`. Then use `man` to learn what the `a`, `l`, and `h` options mean when used with the `ls` command. *Write down what those options do?*
man formats and displays the on-line manual pages. If you specify section, man only looks in that section of the manual. name is normally the name of the manual page, which is typically the name of a command, function, or file. a comes up as all, l comes up as long listing format, and h comes up as human-readable *print sizes in human-readable format*

* Commands can also take *arguments*, which are usually the names of files or locations that you want the command to work with. Try running `ls /` to see what files are in the *root* directory of the filesystem. *What files and directories do you see listed?*
bin   dev  fastboot  lib    media  opt   root  sbin  sys  usr           
boot  etc  home      lib64  mnt    proc  run   srv   tmp  var 

* A Unix filesystem has a few special shortcuts to refer to specific locations. `/` indicates the *root* of the filesystem, meaning the top-most directory in the filesystem hierarchy. Use the `cd` ("change directory") command to move to the root directory. (Hint: Use `man` to look up the `cd` command if you have any issues) *Then run `pwd` and paste the output here:*
I input cd then pwd and came up with: /home/cabox 

* Another special shortcut in Unix is the `~` location. This indicates the *user root* directory, meaning the top-most directory in the hierarchy that comes below your user account. Use `cd` to move to `~`. *Run `pwd` and paste the response here:*
Come back to it?

* Change directory into the `challenge_files` directory. Use `ls` to find only the files with a `.demo` pattern. *How many files do you find?* 
01                       Hillard-Ziemann.user                           
2015_special_stuff.demo  Isadora-Leffler.user                           
Afton-Jast.user          Jaxen-Gleichner.user                           
Aimee-Maggio.user        Jayme-Rodriguez.user                           
Alfonso-Gottlieb.user    Jenni-O'Connell.user                           
Allen-Kemmer.user        Johny-Borer.user                               
Almina-Cormier.user      Kassandra-Barrows.user                         
Alta-Lemke.user          Keely-Hilpert.user                             
Amina-McGlynn.user       Kenyatta-Hickle.user                           
Anabel-Hammes.user       Kiana-Kulas.user                               
Ancel-Conn.user          Kirstin-Hoppe.user                             
Anjali-Halvorson.user    Kwame-Schmitt.user                             
Ardath-Kuvalis.user      Ladonna-Lueilwitz.user                         
Avah-Dickinson.user      Lala-Will.user                                 
Ayaan-Stiedemann.user    Leia-Hudson.user                               
Aylin-Grant.user         Leia-Ziemann.user                              
Bedford-Sipes.user       Lillard-Purdy.user                             
Benita-King.user         Lilly-Kohler.user                              
Benito-Stoltenberg.user  Lissie-Strosin.user                            
Beverlee-Moen.user       Mannie-Ritchie.user                            
Brad-Thiel.user          Masako-Lind.user                               
Brayan-Douglas.user      Melisa-Yundt.user                              
Bria-Satterfield.user    Michelina-Kuphal.user                          
Bridgette-Reichel.user   Minnie-Jacobi.user                             
Britt-Erdman.user        Murdock-Leffler.user                           
Britta-Hammes.user       Mychal-Corkery.user                            
Bryant-Kuhic.user        Nakita-Nader.user                              
Bryton-Aufderhar.user    Nayely-Dare.user                               
Caitlin-Grady.user       Nicholas-Strosin.user                          
Carroll-Hartmann.user    Niles-Runte.user                               
Claudie-McClure.user     Nina-Sporer.user                               
Clemente-Haley.user      Noreta-Steuber.user                            
Cleo-VonRueden.user      Ovid-Bogan.user                                
Codie-Romaguera.user     Randell-Sauer.user                             
Cooper-Reynolds.user     Remy-Renner.user    
Corrie-Bogisich.user     Ronna-Hermann.user                             
Dannielle-Green.user     Rosalind-Wisozk.user                           
Deedee-Jacobson.user     Rosena-Simonis.user                            
Desiree-Marks.user       Sandie-Balistreri.user                         
Deven-Rutherford.user    Sharen-Hansen.user                             
Doyle-Jones.user         Sherrill-Russel.user                           
Dustyn-O'Connell.user    Sherwin-Kovacek.user                           
Elza-Mraz.user           Sherwood-Rath.user                             
Emory-Crona.user         Shyheim-Murazik.user                           
Erin-Walker.user         Siobhan-Kirlin.user                            
Estela-Schultz.user      Tomas-Kutch.user                               
Fernanda-Tromp.user      cloaked-wookie.demo                            
Fletcher-Rice.user       credit_cards.txt                               
Fred-Ryan.user           credit_cards2.txt                              
Genie-Abshire.user       scooter-double-mamba.demo                      
Grace-Tromp.user         serial-numbers                                 
Grant-Cronin.user        test2                                          
Hali-Roob.user           tmp                                            
Harland-Schoen.user      wow                                            
Harrell-Quitzon.user               
* Use the `cd` command to move "up" one directory. *Where are you in the filesystem now?* 
cabox@box-codeanywhere:~$  

* Press the up arrow on your keyboard. *What just happened?*
It cycled through the previous commands. *cd and ls*

* Press the up arrow a few more times. *What do you see?*
It continues to cycle through past commands, I can see my previous moves. 

* Run the `history` command. *What do you see?*
Holy smokes, now I can see all of the previous commands during my experimenting session! Cool.  

### Observing the System

* Discover what account you are logged into using the `whoami` command. *What username are you currently using?*
cabox

* Discover who else is on your system with the `who` command. *Are any other users using your system? If so, list them here:*
cabox    pts/0        Apr  9 16:41 (54.69.152.243) 

* How long has your system been running? Use `uptime` to see, and *paste the result here:*
 17:06:08 up  1:42,  1 user,  load average: 0.00, 0.00, 0.00

* Run `ps aux` and review the results. (Hint: Use `man` to learn more about the `ps` command and options.) *How do you interpret what you see here?*
It displays a lot of information. Seems to bounce between root and cabox a lot in the USER column. The numbers get higher in the PID column. Not entirely sure what it means other than usage between CPU and MEM. 

* Run `top` and review the results. (Hint: You may need to use `ctrl-c` to get out of this app.) *How do you interpret what you see here?*
A lot of information once again, this time it seems to be fluctuating a little, the time seems to be going up in increments of 3 seconds. Perhaps tracking member usage based on Tasks section. VIRT is the sum memory it is using, I wanted to look it up. Very cool!


### Finding and Viewing Files

* Make sure you are in the `challenge_files` directory. Use the `*` wildcard to find all the files that have the word "credit" in the filename. *How many files did you find?*
credit_cards.txt  credit_cards2.txt 

* Use the `more` command to view one of the `credit_cards` files you just discovered. (Hint: Type `q` to quit viewing the file. Press the `spacebar` to page down. Use your keyboard arrows to move up/down.) *What is the date in the file you have viewed?*
Last updated: 01-15-2015

 * Use the `find` command to search for files more effectively. Search the sub-directories under `challenge_files` to find the location of the file named `modi_laboriosam.txt`. *Where is that file located?*
./tmp/modi_laboriosam.txt

* Use the `grep` command to search for text within a file. Use `grep` on all the `.user` files in `challenge_files` to find which files contain "WA" (the abbreviation for Washington state). *How many files did you find?*

* Use the `-r` option of `grep` to *recursively* find the text "Waldo" hidden in a file somewhere under the `challenge_files` directory. *Paste the result showing the file and line where the word "Waldo" shows up.*
serial-numbers/eaque_molestiae.txt:Ut est maiores quia autem. Nisi modi Waldo s                
ed corporis sit explicabo ut est. Et est placeat ea sunt sunt consectetur sunt                 
incidunt. Explicabo vel esse blanditiis dolorem culpa non quia. 

### Pipes and Connecting Commands

* Sometimes it's useful to output the results of a command to a text file for further analysis, reference, or processing. Try running `ls > files.txt`. Notice that the file `files.txt` was created. View that file using `more`. *What do you see in the `files.txt` file?*

* Notice that if you run `ls -alh` in the `challenge_files` directory, the files scroll by very quickly. Sometimes it would be better to get the results in a paginated format. Try running `ls -alh | more`. *Describe what you see when you run `ls -alh | more`.*
When I initiate the more feature I can see a smaller chunk of text, where it isn't as overwhelming and I can load the rest as I choose.

* Earlier, when you viewed the list of active processes on your devbox using `ps aux`, the list was probably really long. You can make this list more manageable by using the pipe (`|`) to filter the results of `ps` using `grep`. Run `ps aux | grep <your_username>` to see what processes are running for your specific user. *Paste the list of processes that reference your username here:*
root       770  0.0  1.2  63876  3344 ?        Ss   16:11   0:00 sshd:                                             
                                                                                                                   
cabox      772  0.0  0.5  64008  1496 ?        S    16:11   0:00 sshd:                                             
                                                                                                                   
cabox      773  0.0  0.3  12920   904 ?        Ss   16:11   0:00 /usr/l                                            
ftp-server                                                                                                         
root       801  0.0  1.2  63876  3340 ?        Ss   16:39   0:00 sshd:                                             
                                                                                                                   
cabox      803  0.0  0.5  64008  1492 ?        S    16:39   0:00 sshd:                                             
                                                                                                                   
cabox      804  0.0  0.3  12920   904 ?        Ss   16:39   0:00 /usr/l                                            
ftp-server                                                                                                         
root      1011  0.0  1.2  63876  3340 ?        Ss   16:52   0:00 sshd:                                             
                                                                                                                   
cabox     1013  0.0  0.5  64008  1500 ?        S    16:52   0:00 sshd:                                             
                                                                                                                   
cabox     1014  0.0  0.7  14376  1880 ?        Ss   16:52   0:00 /usr/l                                            
ftp-server                                                                                                         
root      1034  0.0  1.2  63876  3344 ?        Ss   17:22   0:00 sshd:                                             
                                                                                                                   
cabox     1036  0.0  0.5  64012  1492 ?        S    17:22   0:00 sshd:                                             
                                                                                                                   
cabox     1037  0.0  0.3  12776   864 ?        Ss   17:22   0:00 /usr/l                                            
ftp-server                                                                                                         
root      1053  0.0  1.2  63876  3344 ?        Ss   17:39   0:00 sshd:                                             
                                                                                                                   
cabox     1055  0.0  0.5  64012  1496 ?        S    17:39   0:00 sshd:                                             
                                                                                                                   
cabox     1056  0.0  0.3  12920   948 ?        Ss   17:39   0:00 /usr/l                                            
ftp-server                                                                                                         
root      1261  0.0  1.2  63876  3348 ?        Ss   17:46   0:00 sshd:                                             
                                                                                                                   
cabox     1263  0.0  0.5  64012  1496 ?        S    17:46   0:00 sshd:                                             
                                                                                                                   
cabox     1264  0.0  0.3  12776   856 ?        Ss   17:46   0:00 /usr/l                                            
ftp-server                                                                                                         
root      1485  0.0  1.3  63876  3488 ?        Ss   18:05   0:00 sshd:                                             
                                                                                                                   
cabox     1487  0.0  0.5  64012  1488 ?        S    18:05   0:00 sshd:                                             
                                                                                                                   
cabox     1488  0.0  1.7  20624  4552 pts/0    Ss   18:05   0:00 -bash                                             
root      1693  0.0  1.2  63876  3344 ?        Ss   18:10   0:00 sshd:
priv]                                                                                              
cabox     1695  0.0  0.5  64012  1504 ?        S    18:10   0:00 sshd: cabox@n                     
otty                                                                                               
cabox     1696  0.0  0.3  13048  1004 ?        Ss   18:10   0:00 /usr/lib/open                     
ssh/sftp-server                                                                                    
root      1719  0.0  1.2  63876  3336 ?        Ss   18:22   0:00 sshd: cabox [                     
priv]                                                                                              
cabox     1721  0.0  0.5  64012  1508 ?        S    18:22   0:00 sshd: cabox@n                     
otty                                                                                               
cabox     1722  0.0  0.3  12776   876 ?        Ss   18:22   0:00 /usr/lib/open                     
ssh/sftp-server                                                                                    
root      1723  0.0  1.3  63876  3488 ?        Ss   18:22   0:00 sshd: cabox [                     
priv]                                                                                              
cabox     1725  0.0  0.5  63876  1468 ?        S    18:22   0:00 sshd: cabox@p                     
ts/0                                                                                               
cabox     1726  0.0  1.7  20624  4548 pts/0    Ss   18:22   0:00 -bash                             
cabox     1923  0.0  0.4  15520  1140 pts/0    R+   18:23   0:00 ps aux                            
cabox     1924  0.0  0.2   8816   760 pts/0    S+   18:23   0:00 grep --color=                     
auto cabox                                   