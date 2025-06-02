
# sysinfo-to-csv

A simple Bash script that collects essential Linux system information (IP address, CPU count, RAM size, total disk size, and specific mount point sizes) and exports the results to both CSV and JSON files.

---

## 📋 Features

- Collects:
  - Server IP address
  - Number of CPUs
  - Total RAM
  - Total disk size
  - Optionally checks for disk sizes of common mount points:![image](https://github.com/user-attachments/assets/83b8ebc3-c9af-4c11-9438-ec0bbf8b161e)

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
![image](https://github.com/user-attachments/assets/a06cda59-7639-4500-91bb-10a39db5c00f)

## 🚀 Usage

```bash
chmod +x sysinfo-to-csv.sh
sudo ./sysinfo-to-csv.sh
