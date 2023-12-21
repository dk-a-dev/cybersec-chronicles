### ### Level-10 Solution
```bash
> strings data.txt | grep =
> exit
> ssh bandit.labs.overthewire.org -p 2220 -l bandit10
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code>G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s</code></pre>
</details>
</p>

### Level-10 Explanation
- `strings data.txt | grep =` : Print the printable characters in the file and then print only those lines that contain the `=` character.
- `exit` : Exit the current session.
- `ssh bandit.labs.overthewire.org -p 2220 -l bandit10` : Login to the server with the given credentials.

![cmd output](level-10.png)