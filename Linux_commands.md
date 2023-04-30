![Screenshot 2023-04-30 161420.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/739ea2dc-6243-4aed-81fd-33aaa12eb249/Screenshot_2023-04-30_161420.png)

**Linux for everyone**

1.  **mkdir** → Create directories
    **mkdir -p** → Create parent directories if not created.

2.  **#** → Comments
3.  **pwd** → Present working directory

4.  **cd** → change / catch directory
    **cd or cd ~** → Home directory
    **cd . .** → Go back to the Parent directory
    **cd /** → Go to root directory
    **cd PATH** → change current directory

5.  **mv** → move files/ directories
6.  **cp** → copy a file / directory
7.  **touch** → To Just create a file
8.  **nano | vim ( editor )**
    → **Ctrl + O ( Save ) → Enter → Ctrl + x ( Exit )**
    → **i** ⇒ insert mode
    → **:wq!** ⇒ Save and exit
    → :q! ⇒ Exit

                           [  ***apt install nano
                             apt install vim*** ]

9.  **cat** → View / append / merge Files
    **cat File1 >> File2** → To append the change
    **cat File1** → To see the content
    **cat “File1” “File2” > Files** → Merge Z files

10. **Ping** → Packet Internet Groper → Check network between hosts / Servers

**ping -c 10( Numeric ) IP/URL** → To send Fix Request

\*\* use ctrl + c to stop sending request

- uses ICMP Protocol\*

11. **curl** → Transfer data to / from server
   **curl -o File URL** → To save a file

- _(More secure | More Advanced | Faster)_

12. **wget →** Downloads files from the server anonymously
   **wget - b URL →** To run in background

- ( Parallel downloads vs Opps. of above )

13. **watch →** to send request periodically (by default 2 seconds )
   **watch -n seconds CMD**
   **watch -n 5 url https: // →** Send the curl request to URL every 5 **Seconds.**

14. **echo →** Just to repeat

15. **base 64 →** convert to base64 encoding

   - **echo “Nikhil” | base 64 →** to encode
   - **echo ‘x 64 …’ | base 64** decode → to decode

16. **ps** → to get the PIDs
   **ps auoc** → To get most of the info about a PID

17. **grep** → To catch specific text from a source
   Kubectl get pods | grep Nikhil

18. **Some special characters**

- **>** → To redirect, override
- **>>** → To append, no override
- **user Symbol >** → To stream
- **2 >** → Error redirection

19. **netstat** → To see netwrok related info

- **netstat -at** → list of all tcp ports
- **netstat - au** → list of all UPD ports
- **netstat - et** → list of listening tcp ports
- **netstat - eu** → list of listening UDP ports

20. **rm** → Remove a file
   **rmdir** → “ “ directory

21. **wc -l** → Court the number of lines

22. **ls -l** → returns list of files in long format.

23. **chmod** → change the access mode of a file

**chmod** **reference** **Operations** **mode** **File**
user u + r  
 group g - w
other o = x
u + g + o a -

ex chmod u =x, go = r FIE

24.  **ssh** → Secure shell to connect with a server → ssh user @ HOST → port 22 (by default)

25.  **scp** → copy files between servers, works on SSH → scp user@ HOST1: File user@HOST2: file

26.  **tar** → tope Archieve → t**ar cvf ( compress| verbox | file ) FILE .ta\*** → to compress

                                  → tar xvf  ( extract )   FILE.t2 → to extract

**tar -zcvf (compress ) archive.tgz folder
tar -zxvf (extract) archive.tgz**

27.  **gzip** → to compress a file → **gzip file.txt** —> (o/p) File.txt.gz ( can’t compress a folder sp we use tar )

              →  to decompress a file → **gunzip  file.txr.gz**  —> (o/p) FILE.txt

28.  **alias** → Just like setting a nickname.

29.  **clear** → to clean the screen / window
30.  **history** → to see the history of commands used
31.  **|** → pipe

**CMD 1 ——> Output ——> | ——> input ——> CMD 2
(passes)**
