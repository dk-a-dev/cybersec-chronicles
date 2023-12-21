### Level-13 Solution
refer [medium article](https://david-varghese.medium.com/overthewire-bandit-level-12-level-13-2ec761a88907)
```bash
> mkdir /tmp/devdk/
> cp data.txt /tmp/devdk/dkdata.txt
> cd /tmp/devdk/
> xxd -r dkdata.txt > dkdata // convert hexdump to binary
> file dkdata
> mv dkdata dkdata.gz
> gzip -d dkdata.gz
> file dkdata
> mv dkdata dkdata.bz
> bzip2 -d dkdata.bz
> file dkdata
> mv dkdata dkdata.gz
> gzip -d dkdata.gz
> file dkdata
....
...
...
.
Continuous decompression using different compression algorithms.
gzip using gunzip
bzip2 using bunzip2
tar using tar -xf
using file command to check the file type.
> exit
> ssh bandit.labs.overthewire.org -p 2220 -l bandit13
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code>wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw</code></pre>
</details>
</p>


![cmd output](image.png)