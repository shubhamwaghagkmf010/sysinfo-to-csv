
# sysinfo-to-csv

A simple Bash script that collects essential Linux system information (IP address, CPU count, RAM size, total disk size, and specific mount point sizes) and exports the results to both CSV and JSON files.

---

## 📋 Features

- Collects:
  - Server IP address
  - Number of CPUs
  - Total RAM
  - Total disk size
  - Optionally checks for disk sizes of common mount points:![image](https://github.com/user-attachments/assets/2dbbc781-0a06-454f-99e1-37ed77477645)


  - Sizes of `/data`, `/app`, `/datafiles`, `/dblogs`, and `/logs` if available
  - partition you created (`/Replace-Your-partition`, `/Replace-Your-partition`, `/etc`,)
- Outputs:
  - CSV file (e.g., `/root/192.168.1.100.csv`)
- Automatically names output files based on server IP

---

## 🔧 Requirements

- Linux system
- Bash shell
- Root access (to write to `/root/`)

---
## 📁 Output Files

### 🔹 CSV Output (example)
![image](https://github.com/user-attachments/assets/17688e2d-3d40-40cf-8ed0-a1fa454683a2)

## 🚀 Usage

```bash
chmod +x sysinfo-to-csv.sh
sudo ./sysinfo-to-csv.sh
