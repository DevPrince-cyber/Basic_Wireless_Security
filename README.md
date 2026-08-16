# Wireless Router Security Configuration Lab

## Overview
This lab exercise guides you through verifying initial network connectivity, securing a home or small office wireless network with WPA2-Personal encryption, configuring client wireless settings on a end-user laptop, and validating end-to-end network connectivity after securing the wireless link.

---

## Part 1: Verify Initial Connectivity

### Accessing the Web Browser
To verify baseline connectivity across the network before making configuration changes, navigate to the **Desktop** tab on the laptop and launch the **Web Browser** application.

### Verifying Web Page Access
In the web browser address bar, enter `www.cisco.pka` and press **Enter**. Confirm that the web page successfully loads and displays. This step ensures that baseline IP connectivity and DNS resolution are functioning properly prior to configuring wireless security.

---

## Part 2: Configure Basic Wireless Security

### Accessing the Wireless Router Administration Interface
Open the Web Browser on the laptop and enter the default gateway IP address `192.168.1.1` into the URL bar to access the Wireless Router management interface. When prompted for credentials, enter `admin` as both the username and password to log in.

### Navigating to Wireless Security Settings
Once authenticated to the administrative portal, click on the **Wireless** menu option located in the top navigation bar, and then select the **Wireless Security** sub-menu to view the active security configurations.

### Enabling WPA2 Personal Security
Observe that the security mode is currently set to **Disabled**. For the **2.4 GHz** wireless network, click the security mode dropdown menu and select **WPA2 Personal**. Leave the security mode for both **5 GHz** networks set to **Disabled**.

### Setting the Wireless Passphrase
In the **Passphrase** field for the 2.4 GHz network, enter `Network123` as the pre-shared key (PSK).

### Saving Administrative Settings
Scroll to the bottom of the management page and click **Save Settings** to apply the security policy. After the settings are saved successfully, close the web browser window.

---

## Part 3: Update Wireless Settings on the Laptop

### Opening the Client Wireless Utility
On the laptop **Desktop** tab, locate and click the **PC Wireless** icon to launch the wireless network interface controller (WNIC) configuration utility.

### Scanning and Connecting to the Wireless Network
Select the **Connect** tab within the PC Wireless application to display available wireless networks. Locate the network named **Academy** from the list, select it, and click the **Connect** button.

### Entering the Pre-Shared Key
When prompted for security authentication, enter `Network123` in the Pre-Shared Key field and click **Connect** to establish the encrypted wireless link with the router.

### Closing the Utility
Once the client utility confirms a successful connection and link status, close the **PC Wireless** window.

---

## Part 4: Verify Final Network Connectivity

### Launching the Web Browser
Re-open the **Web Browser** application from the laptop's Desktop tab to perform final post-configuration validation testing.

### Validating Web Resource Accessibility
Enter `www.cisco.pka` into the address bar and verify that the web page loads properly. Successful access confirms that the laptop can communicate securely across the encrypted wireless network to reach destination services.

### Troubleshooting Unsuccessful Connections
If the web page fails to display, open the Wireless Router management page and the laptop **PC Wireless** utility to verify that the SSID and WPA2 pre-shared key (`Network123`) match identically on both devices. Ensure that the laptop has successfully associated with the wireless router and obtained a valid IP address.