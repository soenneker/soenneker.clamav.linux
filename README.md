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

## Licensing and source

This package redistributes official ClamAV binaries, which are licensed under GPL-2.0-only. The NuGet package includes the GPL v2 text, ClamAV's upstream `COPYING.txt`, and the `COPYING/` directory containing notices for bundled third-party components.

The runtime's `SOURCE.txt` identifies its exact upstream binary asset, release, and corresponding source archive. See [Cisco-Talos/clamav releases](https://github.com/Cisco-Talos/clamav/releases) for upstream release materials.
