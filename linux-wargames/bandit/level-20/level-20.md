### Level-20 Solution
```bash
> ls -l bandit20-do
# -rwsr-x--- 1 bandit20 bandit19 7296 Nov 14  2014 bandit20-do
> ./bandit20-do cat /etc/bandit_pass/bandit20
# copy and paste password
```
<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code></code>VxCazJaVykI6W36BkBU0mJTCM8rR95XT</pre>
</details>
</p>

### Level-20 Explanation
we used ./bandit20-do to execute the command cat /etc/bandit_pass/bandit20 as bandit20 user. This is because the file bandit20-do has the setuid bit set. This means that when the file is executed, the process will have the same permissions as the user that owns the file. In this case, the file is owned by bandit20, so we run the command as bandit20. This command gives us the password for the next level.

![cmd output](image.png)