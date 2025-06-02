
# sysinfo-to-csv

A simple Bash script that collects essential Linux system information (IP address, CPU count, RAM size, total disk size, and specific mount point sizes) and exports the results to both CSV and JSON files.

---

## 📋 Features

- Collects:
  - Server IP address
  - Number of CPUs
  - Total RAM
  - Total disk size
  - Sizes of `/data`, `/app`, `/datafiles`, `/dblogs`, and `/logs` if available
  - Please add the partition you created (`/Your-partition`, `/Your-partition`, `/etc`,)
- Outputs:
  - CSV file (e.g., `/root/192.168.1.100.csv`)
  - JSON file (e.g., `/root/192.168.1.100.json`)
- Automatically names output files based on server IP

---

## 🔧 Requirements

- Linux system
- Bash shell
- Root access (to write to `/root/`)

---

## 🚀 Usage

```bash
chmod +x sysinfo-to-csv.sh
sudo ./sysinfo-to-csv.sh
