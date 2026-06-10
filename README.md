# knowledgepress-releases

Official download & release channel for **KnowledgePress** — export Salesforce
Knowledge Articles into clean, print-ready PDFs. (The application source is
maintained privately; this repo hosts only the published, signed build artifacts.)

## Download
Grab **`KnowledgePress.zip`** from the [latest release](https://github.com/beebojones/knowledgepress-releases/releases/latest),
unzip it, and run `KnowledgePress.exe`. Requires Microsoft Edge (ships with Windows).

## Verify your download
Each release publishes `KnowledgePress.zip.sha256` (checksum) and
`KnowledgePress.zip.sig` (signature). To confirm the zip is intact:

```powershell
Get-FileHash .\KnowledgePress.zip -Algorithm SHA256
# compare to the contents of KnowledgePress.zip.sha256
```

KnowledgePress also verifies both the checksum and the signature automatically
before installing any in-app update, and refuses to install if either fails.
