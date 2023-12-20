### ### Level-9 Solution
```bash
> sort data.txt | uniq -c | grep -w 1
> exit
> ssh bandit.labs.overthewire.org -p 2220 -l bandit8
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code>EN632PlfYiZbn3PhVK3XOGSlNInNE00t</code></pre>
</details>
</p>

### Level-9 Explanation
- `sort data.txt | uniq -c | grep -w 1` : Sort the data in the file, count the number of occurrences of each line, and then print only those lines that occur once.
- `exit` : Exit the current session.
- `ssh bandit.labs.overthewire.org -p 2220 -l bandit9` : Login to the server with the given credentials.

![cmd output](level-9.png)