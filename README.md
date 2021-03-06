# Lyrica
A CLI Tool to Scrape Lyrics from Terminal either using Rofi or FZF(default). The script scrapes lyrics from <a href="https://www.azlyrics.com"> A-Z Lyrics </a> using <i>curl</i>, <b>fzf</b> or <b>rofi</b> as a menu and uses <b>bat</b> to display the lyrics.

## Showcasae

<img src="https://github.com/Sidmaz666/lyrica/blob/main/assets/preview.gif" width="100%">

## Dependencies

#### Set the TERM Variable

<b>Rofi</b> will spawn <i>bat or cat</i> in the default Terminal, as set in the TERM Variable in .zshrc, .bashrc , .xinitrc or in the /etc/environment file.

1. curl (for scrapping)
2. sed (for regex)
3. grep (for regex)
4. fzf (for menu)
5. bat  (for displaying lyrics, pager)
6. rofi (for menu-optional)
7. nerd-font (for uicode support-very optional)

## Installation

You can run the script as usual!
                
       ./lyrica Monster
       ./lyrica --rofi

However, if you search for lyric from your terminal or would like to bind lyrica to a <i>keybinding</i> then run the following command to install <b>Lyrica </b><i> system-wide</i>

       sudo cp lyrica /usr/bin/lyrica
                  
                  
# Usage

     [USAGE]: lyrica [SEARCH_QUERY]
     lyrica --rofi To Launch Lyrica With Rofi
                  By Default Menu is set to FZF	       
     lyrica [SEARCH_SONG_NAME] > [LYRIC_FILE_NAME].txt To Download
     lyrica -h | --help To See Usage!

#### Download

     lyrica Dancing in my room > lyrics.txt

# Misc

- Change the default Pager <i>bat</i> to <b>cat</b> by modifying the <b>DISPLAY_LYRIC</b> variable. 
- To change the Rofi Search Prompt Theme, change the variable <b>ROFI_PROMPT</b>. 
- Additional FZF flags can be added by modifying the <b>FZF_PROMPT</b> variable.
- Select the last option, <b>0. Go to Next Page</b> to scrape more lyrics!       



### Licensed under <a href="https://github.com/Sidmaz666/lyrica/blob/main/LICENSE.md"><b>GPL-3.0</b></a>
