### Level-21 Solution
```bash
# open two terminals:

### terminal-1 ###
> ssh bandit20@bandit.labs.overthewire.org -p 2220
# enter with level 20 password
> nc -l 3000
# after connecting to port for another terminal give last level password
# new level password will be displayed in terminal-1

### terminal-2 ###
> ssh bandit20@bandit.labs.overthewire.org -p 2220
# enter with level 20 password
> ./suconnect 3000
# Read: <password from level-20>
# Password matches, sending next password
```

<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code></code>NvEJF7oVjkddltPSrdKEFOllh9V1IBcq</pre>
</details>
</p>

### Level-[level-number] Explanation
1. `nc -l 3000` will open a port on localhost with port number 3000
2. `./suconnect 3000` will connect to port 3000 and send the password for level-21
3. `suconnect` is a binary file which is provided by the challenge

![cmd output](image.png)