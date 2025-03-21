# Nessus


<div align="left">
  <img src="Screenshot 2025-03-19 095551.png" alt="Download" style="max-width: 300px; height: 300px;">
</div>
Downloading Windows Iso for Oracle VM virtualbox


<div align="left">
  <img src="Screenshot 2025-03-21 100745.png" alt="Bridged network" style="max-width: 300px; height: 300px;">
</div>

We use a bridged network so our VM has access to the internet


<div align="left">
  <img src="Screenshot 2025-03-19 161525.png" alt="VM&Nessus" style="max-width: 300px; height: 300px;">
</div>

<div align="left">
  <img src="Screenshot 2025-03-19 165447.png" alt="IPaddress" style="max-width: 400px; height: 400px;">
</div>

Use "ipconfig" to find the IP address of the machine

<div style="display: flex;">
  <div align="left">
    <img src="Screenshot 2025-03-20 061340.png" alt="firewall" style="max-width: 400px; height: 400px;">
  </div>

  <div align="left">
    <img src="Screenshot 2025-03-20 061417.png" alt="firewall" style="max-width: 400px; height: 400px;">
  </div>

  <div align="left">
    <img src="Screenshot 2025-03-20 061218.png" alt="firewall" style="max-width: 400px; height: 400px;">
  </div>
</div>

turn off firewall to allow the nessus to scan the system

<div align="left">
  <img src="Screenshot 2025-03-20 075929.png" alt="remote reg 6" style="max-width: 400px; height: 400px;">
</div>

Enabiling remote registry and setting it to automatic


<div align="left">
  <img src="Screenshot 2025-03-20 063826.png" alt="Scan" style="max-width: 400px; height: 400px;">
</div>

Credentialed scan to allow the scan to futher into our target machine

<div align="left">
  <img src="Screenshot 2025-03-20 063320.png" alt="Scan" style="max-width: 400px; height: 400px;">
</div>

inputting IP address of target


<div align="left">
  <img src="Screenshot 2025-03-20 082051.png" alt="vulnerabilities" style="max-width: 400px; height: 400px;">
</div>

vulnerabilities/information a out sysytem

<div align="left">
  <img src="Screenshot 2025-03-20 082417.png" alt="SMB" style="max-width: 400px; height: 400px;">
</div>

Medium risk- allowing for a MITM attack- if data is being sent over that port

