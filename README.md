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
  
- Don't forget to add never_kill_your_time on startup application of ubuntu the location of installation is `/bin/never_kill_your_time`
- Time format in json file is "hh:mm", where the acceptable range of "hh" is 0-23, and of "mm" is 0-59. (Thank You [tarunvelli](https://github.com/tarunvelli))
- I know editing the json file is a buzzkill. I will fix that as soon as I can. Thank You.
- Or you could contribute. If you can please help me :) 

## Yahoo I am Happy
- Thank you for using never kill your time
- I am not dedicated to making this app easier to user. Do you know why? I like it when people play around with code. 
- Happy Coding !!! 


