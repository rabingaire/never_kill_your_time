# never kill your time
A simple script that creates push notification on Ubuntu to remind your routine.
![Screenshot](./screenshot.jpg)

## How to install
- Clone the repository
- Add your Routine on the file name routine.json inside never_kill_your_time folder. Example of the routine is given below:

  ```json
  [
    {
      "time":"15:00",
      "title":"Learn!",
      "body":"learn python"
    }
  ]
  ```

- Run the script given below inside never_kill_your_time folder

  ```bash
  chmod a+x install.sh
  sudo ./install.sh
  ```

- After installation you can run the script just by simply typing

  ```bash
   ~ $ never_kill_your_time  
  ```

## Post installation

-  to add routine

` sudo never_kill_your_time add "time" "title" "body" `

time should be in "hh:mm"

time, title and body should be enclosed in quotation marks " "

example
```bash
~ $ sudo never_kill_your_time add "20:45" "music" "listen to music"
```

- to update routine

` sudo never_kill_your_time update "time" "new title" " new body" `

time should be in "hh:mm"

time, title and body should be enclosed in quotation marks " "

time should be pre existing in json file, "new title" and "new body" will be the  new title and new body for that time.

example if the json already contains
>>{
>>"time":"10:45",
>>"title":"music",
>>"body":"listen to music"
>>}

```bash
~ $ sudo never_kill_your_time update "10:45" "study" "study hard"
```
will modify it to  
>>{
>>"time":"10:45",
>>"title":"study",
>>"body":"study hard"
>>}

- to delete routine

` sudo never_kill_your_time delete "time" `

time should be in "hh:mm"

will delete the entry corresponding to that particular time from the json file

example
```bash
~ $ sudo never_kill_your_time delete "10:45"
```

- Don't forget to add never_kill_your_time on startup application of ubuntu the location of installation is `/bin/never_kill_your_time`
- Once the script hs been installed through install.sh, the json file in the repo will become redundent, as all the edits happen to /bin/routines.json. hence after installation always run the script by
```bash
 ~ $ never_kill_your_time  
```
to ensure that the right json file is being loaded
- Time format in json file is "hh:mm", where the acceptable range of "hh" is 0-23, and of "mm" is 0-59. (Thank You [tarunvelli](https://github.com/tarunvelli))
- Or you could contribute. If you can please help me :)

## Yahoo I am Happy
- Thank you for using never kill your time
- I am not dedicated to making this app easier to user. Do you know why? I like it when people play around with code.
- Happy Coding !!!
