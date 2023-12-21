### Level-16 Solution
```bash
> openssl s_client -connect localhost:30001
> // give last level password
> // press enter
> exit
> ssh bandit16@bandit.labs.overthewire.org -p 2220
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code>JQttfApK4SeyHwDlI9SXGR50qclOAil1</code></pre>
</details>
</p>

### Level-16 Explanation
"openssl s_client" is used to connect to a secure socket layer (SSL) server. The "-connect" flag is used to specify the host and port to connect to. In this case, we are connecting to localhost on port 30001. The password from the previous level is then entered. The connection is then closed with "exit". The ssh command is then used to connect to the bandit16 user on the bandit.labs.overthewire.org server on port 2220. The password is the password obtained from the previous level.
we can also add -quiet to the openssl command to remove the extra output like ssl certificate and stuff.

![cmd output](image.png)