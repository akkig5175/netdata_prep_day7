# netdata_prep_day7
# 🖥️ Task 7 - Monitor System Resources Using Netdata

## 📌 Objective
Install **Netdata** and visualize **system & application performance metrics** in real-time.

---

## 🛠 Tools Used
- Netdata (Free, open-source monitoring tool)
- Docker

---

## 🚀 Steps Performed

1. **Pulled & ran Netdata Docker container**  
   ```bash
   docker run -d --name=netdata \
     -p 19999:19999 \
     --cap-add SYS_PTRACE \
     --security-opt apparmor=unconfined \
     netdata/netdata
http://localhost:19999
