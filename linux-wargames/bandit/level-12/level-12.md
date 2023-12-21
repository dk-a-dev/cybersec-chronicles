### Level-12 Solution
```bash
> alias rot13="tr 'A-Za-z' 'N-ZA-Mn-za-m'"
> cat data.txt | rot13
> exit
> ssh bandit.labs.overthewire.org -p 2220 -l bandit12
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code>JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv</code></pre>
</details>
</p>

### Level-12 Explanation
- `alias rot13="tr 'A-Za-z' 'N-ZA-Mn-za-m'"` : Create an alias for the `tr` command.
Here 'A-Z a-z' is the range of characters to be replaced and 'N-Z A-M n-z a-m' is the range of characters to be replaced with.
Note: I had spaced the ranges to make it more readable.
- `cat data.txt | rot13` : Pipe the contents of the file to the `rot13` command.
- `exit` : Exit the current session.
- `ssh bandit.labs.overthewire.org -p 2220 -l bandit12` : Login to the server with the given credentials.
![cmd output](image.png)