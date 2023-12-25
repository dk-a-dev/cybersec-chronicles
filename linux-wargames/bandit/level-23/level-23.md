### Level-23 Solution
```bash
> cat /etc/cron.d/cronjob_bandit23
> cat /usr/bin/cronjob_bandit23.sh
# Follow the given instructions
>  myname=$(whoami)
>  mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)
> echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"
> cat /etc/bandit_pass/$myname > /tmp/$mytarget
Run all given commands as it
```

<p>
<details>
<summary>Password (Spoiler Alert).</summary>
<pre><code></code>QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G</pre>
</details>
</p>

![cmd output](image.png)