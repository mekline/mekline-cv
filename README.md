# mekline-cv

I didn't maintain my CV for 2 years (away at COS!), and on return realized I might literally die if I had to maintain a manual CV ever again. 
So I've attempted a machine-readable version that just lets me add new entries to some CSVs!

Many other people have had this idea! I tested two existing R packages:

[datadrivencv](https://github.com/nstrayer/datadrivencv) 

[vitae](https://cran.r-project.org/web/packages/vitae/index.html)

The resulting CVs were cool and pretty, but also imposed a lot of formatting that I didn't want, since one of my goals was to send the resulting raw HTML to my website, to be formatted along with everything else there. Since those packages rely on templates, the raw MD that was left after removing those templates was not ideally formatted for knitting on its own :) 

Also, I wanted to drop a list of DOIs in and never ever format a citation ever again. So I pull from [rcrossref](https://www.rdocumentation.org/packages/rcrossref/versions/1.1.0), which works beautifully except for one paper (which has a consortium author instead of individual humans).

The results you can see in this repo, as standalone HTML or PDF documents. I prioritized a readable document that only used markdown to display the entries, though I did cave and use `<br>` tags to help with spacing.

You can also follow [this link](https://www.melissaklinestruhl.com/cv/) to see the resulting page on my website, source code [here](https://github.com/mekline/mekline.github.io). This is done by simply dumping the non-redundant lines of the html file from this repo into a file called `cv.md`, with the appropriate frontmatter to work with the rest of the Jekyll site ([Direct link](https://github.com/mekline/mekline.github.io/blob/main/cv.md)).


