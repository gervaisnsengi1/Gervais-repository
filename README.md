Cloud-Managed NVAs vs Third-Party NVAs: Networking and Challenges

This project compares Cloud Service Provider (CSP) managed Network Virtual Appliances (NVAs) with third-party NVAs, focusing on networking capabilities, failover performance, and optimization opportunities.

🎯 Objectives
  =============
  Evaluate networking capabilities across CSPs
  Establish an IPSec VPN tunnel between Google Cloud Platform (GCP) and Microsoft Azure
  Optimize routing functionalities
  Measure network convergence and failover times
  Suggest areas of improvement for CSPs
  
🛠️ Tools & Technologies
   ======================

  Google Cloud Platform (GCP)
  Microsoft Azure
  Visual Studio Code (VS Code)
  Terraform
  
🧪 Experiments & Scenarios
 ===========================
 
Scenario 1 (Cloud-Managed NVAs) & Diagram:


Initiated pings between VMs on GCP and Azure via IPSec tunnel
Simulated VPN tunnel failure
Observed 76.7% packet loss during failover




<img width="400" height="250" alt="image" src="https://github.com/user-attachments/assets/ae129e34-9c1a-4ebe-8b45-e9a1cabd23ed" />



Scenario 2 (Third-Party NVAs - FortiGate) & Diagram:

Simulated Active FortiGate failure on Azure
Measured failover time for Passive FortiGate takeover
Enhanced convergence using BFD protocol and BGP timer manipulation

<img width="400" height="250" alt="image" src="https://github.com/user-attachments/assets/55e65811-bf99-456b-a8f9-74a6fdd61696" />



📊 Results & Analysis
=====================

  CSP-managed NVAs experienced significant packet loss and slower failover
  Third-party NVAs (FortiGate) provided faster convergence and more robust failover handling
  Optimization techniques (BFD + BGP tuning) further improved performance

📌 Conclusion
=============
Third-party NVAs offer superior reliability and control in multi-cloud networking compared to CSP-managed NVAs. However, they introduce additional complexity in setup and management.
