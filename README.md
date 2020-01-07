# California Gothic
In 1953, California standardized the state flag in law.  Section 420 of the Government Code says:

```
The general design and the details of the Bear Flag, excluding colors, 
shall correspond substantially with the following representation
```
![California Flag](https://raw.githubusercontent.com/mattlag/California-Gothic/master/Images/California_Flag.png)
...and includes this low res sketch of the flag itself.  

### But hark!
No mention of a specific typeface to use for the iconic CALIFORNIA REPUBLIC text along the bottom of the flag.  
Not even a family... or even serif / sans-serif.  Just "correspond substantially". Okay.

Long story short, this project aims to reverse-engineer a typeface based on high-resolution scans
of the letter forms from [the original 1953 law](https://raw.githubusercontent.com/mattlag/California-Gothic/master/Images/State_Law_Page_2639.png).


# Info
### Download the font files from [mattlag.com/californiagothic](https://www.mattlag.com/californiagothic)
v2.0 is out, it is a complete re-drawing of all glyphs, and includes 415 characters from the following ranges:
 - Basic Latin (U+0020 - U+007E)
 - Latin Supplement (U+00A0 - U+00FF)
 - Latin Extended-A (U+0100 - U+017F)
 - Combining Diacritical Marks (U+0300 - U+036F)
 - General Punctuation (U+2000 - U+206F)

![OFL Logo](https://scripts.sil.org/cms/sites/nrsi/media/OFL_logo_circ_color.png) | California Gothic is released under the SIL Open Font License, which you can read about in OFL.txt and 
OFL-FAQ.txt in this project.


# Build Process
This is a passion project of mine, but I also used designing this typeface to help me test scenarios for 
Glyphr Studio ([Website](https://www.glyphrstudio.com) - [GitHub](https://github.com/glyphr-studio)) 
which is *another* passion project of mine.  All the source files are included in this repo, but it may 
not look like "normal" typeface design source files.  So, here is an overview of the process of how this 
typeface was built:

 1. Design base glyphs in Adobe Illustrator
    - Designed at full Em size (2048) Split into files for Letters and Symbols
    - Copy those two files and flatten / combine all shapes
 2. Export each glyph as an individual SVG file
 3. Import each SVG glyph into a Glyphr Studio project
    - Use the Diacritical Glyph Generator global action to make diacritics
    - Flatten some of the resulting glyphs generated by the diacritical glyph generator
    - Inspect each character and make sure all points are rounded to whole numbers
    - Use the All Caps Font global action to copy capitals to lower-case characters
    - Kern everything
 4. Export a SVG Font (to retain Kern information) and open that with Font Forge
    - Edit Metadata
    - Export fonts (OTF, TTF, SVG, EOT, WOFF, and WOFF2 formats)

All of the files for each of these stages are available in the 
[Working_Files](https://raw.githubusercontent.com/mattlag/California-Gothic/master/Working_Files) folder.


# Hey, it's me!
HMU with any questions or comments!

| ![Matthew LaGrandeur's picture](https://1.gravatar.com/avatar/f6f7b963adc54db7e713d7bd5f4903ec?s=70) |

| [Matthew LaGrandeur](http://mattlag.com/)

matt[at]mattlag[dot]com |
