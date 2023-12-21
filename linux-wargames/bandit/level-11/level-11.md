### Level-11 Solution
```bash
> base64 -d -i data.txt
> exit
> ssh bandit.labs.overthewire.org -p 2220 -l bandit11
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code>6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM</code></pre>
</details>
</p>

### Level-11 Explanation
- `base64 -d -i data.txt` : Decode the given base64 encoded data. -d for decode and -i for ignore non-alphabetic characters.
- `exit` : Exit the current session.
- `ssh bandit.labs.overthewire.org -p 2220 -l bandit11` : Login to the server with the given credentials.
![cmd output](image.png)