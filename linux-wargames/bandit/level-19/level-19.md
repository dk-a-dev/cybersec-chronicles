### Level-19 Solution
```bash
> ssh bandit18@bandit.labs.overthewire.org -p cat readme
# give prev password
> copy the obtained password
#################OR###############
> ssh bandit18@bandit.labs.overthewire.org -p 2220 /bin/bash --norc 
# norc means Don’t read the ~/.bashrc initialization file in an interactive shell.
# enter prev password
> cat readme
# copy the obtained password
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code></code>awhqfNnAbc1naukrpqDYcF95h7HoMTrC</pre>
</details>
</p>

### Level-19 Explanation
1. ssh into the server with the given port number and username
2. use the `cat` command to read the contents of the `readme` file
3. copy the obtained password

![cmd output](image.png)