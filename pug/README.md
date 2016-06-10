#Pug

## Sublime text builder

create DockerPug.sublime-build file in 

    /home/$USER/.config/sublime-text-3/Packages/User/DockerPug.sublime-build

put:
  
    {
      "shell_cmd": "docker run --rm --volume=\"/home/$USER:/home/$USER\" --workdir=\"$file_path/\" leandrosouza/pug pug \"$file\""
    }


