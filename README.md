# markdown-resume
A markdown version of my resume that I can update in a single place.

I will utilize github workflows to convert it to other popular formats such as .PDF, HTML, or .DOCX on demand.

Dependencies:
- Windows Computer
- Powershell
- Chocolatey
- pandoc/MIKTeX

Running WSL 2.0 Ubuntu 20.04 on Windows 11
sudo apt install pandoc texlive-latex-recommended texlive-xetex texlive-luatex pandoc-citeproc wkhtmltopdf

pandoc --variable urlcolor=cyan resume.md -o resume.pdf
pandoc resume.md -s -o resume.html
pandoc resume.md -s -o resume.docx
