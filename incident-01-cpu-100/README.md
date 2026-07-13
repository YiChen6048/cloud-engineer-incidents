## Investigation

### 1. Check CPU usage

```bash
top
```

CPU utilization was close to 100%.



![top](screenshots/top.png)

---

### 2. Identify the process 

```bash
ps aux --sort=-%cpu
```

Found `python3 cpu_hog.py` consuming 99% CPU.

![ps-aux](screenshots/ps-aux.png)

---

### 3. Terminate the process

```bash
kill 1234
```


![kill](screenshots/kill-process.png)

---

### 4. Verify recovery

```bash
top
```

CPU utilization returned to normal.


![recovery](screenshots/cpu-recovered.png)