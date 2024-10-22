# **Podman Desktop Setup Guide**

## **Prerequisites**

Before installing Podman Desktop, ensure the following prerequisites are met:

1. **Virtualization (Windows Only)**: Ensure that your system supports hardware virtualization and it is enabled in your BIOS/UEFI settings. This is necessary for running containers efficiently.  
2. **Podman Engine (Linux Only)**: If you're using Linux, it's recommended to install Podman first. Podman Desktop can run without the Podman CLI on Windows/macOS, but the engine may be required if you want to execute Podman commands in the terminal.

---

## **Installation Instructions**

### **1\. Windows**

#### **Step 1: Download Podman Desktop Installer**

* Go to the official Podman Desktop GitHub repository or website.  
* Download the Windows Installer.

#### **Step 2: Install Podman Desktop**

* Run the installer `.exe` file.  
* Follow the prompts to install Podman Desktop.  
  * The installer will take care of setting up a virtual machine for running containers (typically with WSL2, but can also use a lightweight VM if needed).

#### **Step 3: Configure Podman Desktop**

* Launch Podman Desktop.  
* Under **Preferences**, you can adjust settings such as:  
  * **Virtualization backend**: Choose between WSL2 or the default lightweight VM.  
  * **Podman CLI**: Ensure the CLI is configured correctly, or Podman Desktop will handle it automatically.

#### **Step 4: Start Using Podman Desktop**

* Once installed, you can manage containers, images, volumes, and even Kubernetes clusters through the user interface.  
* You can also use **Podman CLI** in the terminal to create and manage containers, as Podman Desktop integrates smoothly with WSL2.

---

### **2\. macOS**

#### **Step 1: Download Podman Desktop Installer**

* Visit the official Podman Desktop website.  
* Download the macOS Installer (this will provide a `.dmg` file).

#### **Step 2: Install Podman Desktop**

* Open the downloaded `.dmg` file.  
* Drag and drop Podman Desktop into your `Applications` folder.

#### **Step 3: Configure Podman Desktop**

* Open Podman Desktop from `Applications`.  
* The application will set up a virtual machine using `qemu` to run Linux-based containers.  
  * You can configure virtual machine settings such as memory and CPU allocation from the **Preferences** menu.

#### **Step 4: Start Using Podman Desktop**

* Once the setup is complete, Podman Desktop is ready to manage containers and images.  
* Use the graphical interface to interact with your container environment or the **Podman CLI** to run commands in the terminal.

---

### **3\. Linux**

#### **Step 1: Install Podman**

* Podman Desktop relies on the Podman engine to manage containers on Linux. First, install Podman via your package manager:

**For Debian/Ubuntu-based systems**:

`sudo apt-get update`  
`sudo apt-get install -y podman`

**For Fedora**:

`sudo dnf install -y podman`

**For Arch Linux**:

`sudo pacman -S podman`

Refer to the Podman installation guide for detailed instructions specific to your distribution.

#### **Step 2: Download Podman Desktop**

* Go to the Podman Desktop GitHub releases page and download the appropriate `.AppImage` file for your Linux system.

#### **Step 3: Make the AppImage Executable**

`chmod +x podman-desktop-linux-x86_64.AppImage`

#### **Step 4: Run Podman Desktop**

* Execute the AppImage:

`./podman-desktop-linux-x86_64.AppImage`

#### **Step 5: Configure Podman Desktop**

* Once launched, Podman Desktop will detect your installed Podman engine.  
* From the **Preferences** section, configure additional settings such as network settings and virtual machine support (if needed).

#### **Step 6: Start Using Podman Desktop**

* Now, you can manage containers and images using the GUI or through the terminal with the **Podman CLI**.

---

