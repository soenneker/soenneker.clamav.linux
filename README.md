[![](https://img.shields.io/nuget/v/soenneker.clamav.linux.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.clamav.linux/)

# Soenneker.Clamav.Linux

The official ClamAV command-line distribution packaged for Linux x64 .NET applications.

```bash
dotnet add package Soenneker.Clamav.Linux
```

The package copies the ClamAV runtime beneath the application output directory:

```text
Resources/linux-x64/clamav/
```

This package contains Linux x64 assets only. Most applications should reference `Soenneker.Clamav.Util`, which selects the correct platform, manages virus definitions, and invokes `clamscan` through a managed API.

The binaries come from the official [Cisco-Talos/clamav releases](https://github.com/Cisco-Talos/clamav/releases) and are distributed under GPL-2.0-only.
