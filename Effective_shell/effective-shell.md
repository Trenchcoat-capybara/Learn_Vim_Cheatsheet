# Effective Shell

## Chapter 1 - Flying the Command Line

Shortcut    Effect  
ctrl + a    go to the beginning of the line.  
ctrl + e    go to the end of the line  
alt + b     move back one word.  
alt + f     move forward one word.  
ctrl + w    delete from beginning of word to cursor.  
alt + d     delete the next word to the right.  
    there are different delete functions, the two use different ones.  
ctrl + u    delete everything from the beginning of the line to the cursor.  
ctrl + k    delete from cursor to end of line.  
ctrl + _    undo most recent change.  

### search commands

Shortcut    Effect  
ctrl + r    activate search backwards prompt in your shell. To find your last mkdir, press ctrl + r, write mkdir, then press ctrl+r again.  
enter       return to regular prompt from search prompt.  
ctrl + s    activate search forward prompt.  
ctrl + g    cancel the current search completely.  

### Useful shortcuts

Shortcut    Effect  
ctrl + l    clear the screen, but don't touch history.  
alt + t     transpose the last two words before the cursor, switching their place.  
ctrl + t    transpose the two letters before the cursor.  
history     opens your history numbering the entries. by typing !# you can rerun command #.  
bindkey     show a list of the current keybinds.  

### pipeline commands

command     function  
sort        sort the input.  
xclip       copy to clipboard. use -o flag to fetch from clipboard.  
uniq        keep only unique lines.  
sed         's/Hello/Goodbye/' Substitute Hello for Goodbye.  
wc          word count, returns lines, words, characters.  
rev         reverse the input.  
less        get a good overview.  
>           add to a place, usually a file. will remove what is in the file.  
>>          append to a place.  
2>&1        take the standard error (2) and pipe it to standard output (1).  

## Chapter 3 - Finding Files and Folders

### Commands
find    *options    starting-point  expression*  
    options - change how find works.  
    starting-point - set find perimeter. the only required argument.  
    expression - more complex patters.  
        -type   -   d for directort, f for files, see man pages for more.  
        -name   -   insert name that is being searched for, use of wildcards possible.  
        -iname  -   case insensitive name flag.  
        -or     -   used to bind two expressions, if either fits show result. "And" is the standard if you use two expressions.  
        -not    -   use to exclude the following expression.  
        -delete -   delete the returned files, don't use it.  

