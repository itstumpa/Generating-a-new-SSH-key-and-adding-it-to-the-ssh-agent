# Generating-a-new-SSH-key-and-adding-it-to-the-ssh-agent


ssh-keygen -t ed25519 -C "your_email@example.com"

$ clip < ~/.ssh/id_ed25519.pub
# Copies the contents of the id_ed25519.pub file to your clipboard

Notes:

With Windows Subsystem for Linux (WSL), you can use clip.exe. Otherwise if clip isn't working, you can locate the hidden .ssh folder, open the file in your favorite text editor, and copy it to your clipboard.
On newer versions of Windows that use the Windows Terminal, or anywhere else that uses the PowerShell command line, you may receive a ParseError stating that The '&lt;' operator is reserved for future use. In this case, the following alternative clip command should be used:
$ cat ~/.ssh/id_ed25519.pub | clip
# Copies the contents of the id_ed25519.pub file to your clipboard



Details:
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
