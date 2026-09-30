# 🎮 Can I Run It?

A sleek, lightweight Windows desktop application that automatically detects your PC's hardware and compares it against the system requirements of any game on Steam. Stop guessing if you can run a game before buying it!

## ✨ Features
- **Auto-Hardware Detection:** Uses Windows WMI to instantly fetch your actual CPU, GPU, total RAM, OS, and available storage. No manual typing required.
- **Steam Store API Integration:** Live search with auto-complete for any game on the Steam catalog.
- **Side-by-Side Comparison:** Displays your PC specs right next to the game's Minimum and Recommended requirements.
- **Color-Coded Verdict:** Instantly tells you if your specs are good to go (Green), uncertain/medium (Yellow), or lacking (Red).
- **Portable & Fast:** Distributed as a standalone executable—no installation required.

## 🚀 Download & Run
1. Go to the [Releases](../../releases/latest) tab.
2. Download the latest `CanIRunIt.exe`.
3. Double-click the file to run it! 
*(Requires Windows 10/11 64-bit and an active internet connection).*

## 🛠️ Tech Stack
- **Framework:** .NET 9.0 (Windows Presentation Foundation)
- **Language:** C#
- **Hardware API:** `System.Management` (WMI)
- **Data Source:** Steam Public Storefront API

## 💻 How to Build Locally
If you want to compile the source code yourself:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/canirunit.git
   ```
2. Navigate to the project directory:
   ```bash
   cd canirunit
   ```
3. Run the app directly:
   ```bash
   dotnet run
   ```
4. Or publish a standalone executable:
   ```bash
   dotnet publish -c Release -r win-x64 --self-contained true -p:PublishSingleFile=true
   ```

## 🤝 Contributing
Pull requests are welcome! Feel free to open an issue if you have ideas for new features (like integrating a GPU benchmark database) or if you spot a bug.
