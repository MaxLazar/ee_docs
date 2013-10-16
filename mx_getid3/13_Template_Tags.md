### {exp:mx_getid3}
**JPEG:**

    {exp:mx_getid3 file='/IMG00018-20100929-1318.jpg'}
        {jpg}
            <p>Size: {height}x{width}</p>
            <p>Made by: {make} {model}</p>
            <p>Date: {datetime}</p>
            <p>Software: {software}</p>
        {/jpg}
    {/exp:mx_getid3} 

**OUTPUT**

    Size: 1600x1200
    
    Made by: Research In Motion BlackBerry 9000
    
    Date: 2010:09:29 13:17:42
    
    Software: Rim Exif Version1.00a

**MP3:**

    {exp:mx_getid3 file='Closer To The Edge.mp3'}
        <p>File Name: {filename}</p>
        <p>Length: {playtime_seconds}</p>
        <p>Playtime: {playtime_string}</p>
    
        {tags_html}
            <p>Title: {title}</p>
            <p>Artist: {artist}</p>
            <p>Album: {album}</p>
            <p>Year: {year}</p>
            <p>Genre: {genre}</p>
        {/tags_html}
    {/exp:mx_getid3} 

**OUTPUT**

    File Name: Closer To The Edge.mp3  
 
    Length: 270.288845502   

    Playtime: 4:30  

    Title: Closer To The Edge   

    Artist: 30 Seconds To Mars 
 
    Album: We Love Winter 2011 
 
    Year: 2011  

    Genre: Pop 

### Parameters ###


#### file ####
Path to file (**full PATH**! not URL)

#### refresh ####
Refresh is the number of minutes between cache refreshes.

#### debug ####
Tell the true - description for all tags which you can use with getID3 library can take more time than writing this plugin. So , if you want to see available tags for target file, just add debug parameter to tag.

    debug = "on"
 
> **IMPORTANT:** Variables can be Single or Pairs.