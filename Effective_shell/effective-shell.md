# Effective Shell

## Chapter 1 - Flying the Command Line

Shortcut    Effect\n
ctrl + a    go to the beginning of the line.\n
ctrl + e    go to the end of the line\n
alt + b     move back one word.\n
alt + f     move forward one word.\n
ctrl + w    delete from beginning of word to cursor.\n
alt + d     delete the next word to the right.\n
    there are different delete functions, the two use different ones.\n
ctrl + u    delete everything from the beginning of the line to the cursor.\n
ctrl + k    delete from cursor to end of line.\n
ctrl + _    undo most recent change.\n

### search commands

Shortcut    Effect\n
ctrl + r    activate search backwards prompt in your shell. To find your last mkdir, press ctrl + r, write mkdir, then press ctrl+r again.\n
enter       return to regular prompt from search prompt.\n
ctrl + s    activate search forward prompt.\n
ctrl + g    cancel the current search completely.\n

### Useful shortcuts

Shortcut    Effect\n
ctrl + l    clear the screen, but don't touch history.\n
alt + t     transpose the last two words before the cursor, switching their place.\n
ctrl + t    transpose the two letters before the cursor.\n
history     opens your history numbering the entries. by typing !# you can rerun command #.\n
bindkey     show a list of the current keybinds.\n

### pipeline commands

command     function\n
sort        sort the input.\n
xclip       copy to clipboard. use -o flag to fetch from clipboard.\n
uniq        keep only unique lines.\n
sed         's/Hello/Goodbye/' Substitute Hello for Goodbye.\n
wc          word count, returns lines, words, characters.\n
rev         reverse the input.\n
less        get a good overview.\n
>           add to a place, usually a file. will remove what is in the file.\n
>>          append to a place.\n
2>&1        take the standard error (2) and pipe it to standard output (1).\n

## Chapter 3 - Finding Files and Folders

### Commands
find    *options    starting-point  expression*\n
    options - change how find works.\n
    starting-point - set find perimeter. the only required argument. \n
    expression - more complex patters. \n
        -type   -   d for directort, f for files, see man pages for more.\n
        -name   -   insert name that is being searched for, use of wildcards possible.\n
        -iname  -   case insensitive name flag.\n
        -or     -   used to bind two expressions, if either fits show result. "And" is the standard if you use two expressions.\n
        -not    -   use to exclude the following expression.\n
        -delete -   delete the returned files, don't use it.\n

