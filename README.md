# miniature-funicular
Web site content and stuff for freeshitter.party

To build this site, do something like this:

```bash
mkdir bin
curl -s https://rgz.ee/bin/ssg > bin/ssg
curl -s https://rgz.ee/bin/Markdown.pl > bin/Markdown.pl
chmod +x bin/ssg bin/Markdown.pl

rm -rf site; mkdir site

PATH="$PWD/bin:$PATH"
bin/ssg . site 'freeshitter.party' 'https://freeshitter.party'
```
