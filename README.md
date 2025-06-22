# gcp-vpc-compute-lab

# GCP Lab: Integrating Compute Engine with VPC Network

## 🧪 Objective
Set up a custom VPC and deploy virtual machines (VMs) within it using the Google Cloud Console.

---

## 🔧 Steps

### 1. Create a Custom VPC Network
- Go to **VPC network ➜ VPC networks ➜ Create VPC network**
- Name it `my-custom-vpc`
- Set Subnet creation mode to **Custom**
- Add subnet (e.g. `subnet-a`, region: `us-central1`, IP range: `10.0.0.0/24`)
- Click **Create**

---

### 2. Create VM Instances in VPC
- Go to **Compute Engine ➜ VM instances ➜ Create instance**
- Name the VM `vm-1`
- Choose region and zone that match your subnet
- Under Networking ➜ **Network interface**, select your `my-custom-vpc` and subnet
- Leave other defaults or customize machine type
- Click **Create**

Repeat for additional VMs if needed.

---

## ✅ Outcome
You now have VM instances deployed inside your custom VPC network.

---

## 📌 Notes
- You can SSH into the VM directly via the GCP console
- To add firewall rules or connect instances, go back to VPC settings
