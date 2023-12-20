### Level-6 Solution
```bash
> find . -size 33c -user bandit7 -group bandit6 | grep bandit7
> cat ./var/lib/dpkg/info/bandit7.password
> exit
> ssh bandit.labs.overthewire.org -p 2220 -l bandit1
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code>z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S</code></pre>
</details>
</p>

### Level-5 Explanation
- find . -size 33c -user bandit7 -group bandit6 | grep bandit7 // Find all files in the current directory that are of size 33 bytes and are owned by user bandit7 and group bandit6 and then match results for bandit7.
- cat ./var/lib/dpkg/info/bandit7.password // Read the contents of the file.
- `exit` : Exit the current session.
- `ssh bandit.labs.overthewire.org -p 2220 -l bandit7` : Login to the server with the given credentials.

![cmd ss as proof](level-7.png)