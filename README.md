# ffind
[![Go Reference](https://pkg.go.dev/badge/github.com/f0x4n6/ffind.svg)](https://pkg.go.dev/github.com/f0x4n6/ffind)
[![Go Report Card](https://goreportcard.com/badge/github.com/f0x4n6/ffind?style=flat-square)](https://goreportcard.com/report/github.com/f0x4n6/ffind)
[![Release](https://img.shields.io/github/release/f0x4n6/ffind.svg?style=flat-square)](https://github.com/f0x4n6/ffind/releases/latest)

Find forensic artifacts in mount points or the live system.

```console
go install github.com/f0x4n6/ffind@latest
```

## Usage
```console
$ ffind [-rcsuqhv] [-H CRC32|MD5|SHA1|SHA256] [-C CSV] [-Z ZIP] [MOUNT ...]
```

Available options:

- `-H` Hash algorithm
- `-C` CSV listing name
- `-Z` Zip archive name
- `-r` Relative paths
- `-c` Volume shadow copy
- `-s` System artifacts only
- `-u` User artifacts only
- `-q` Quiet mode
- `-h` Show usage
- `-v` Show version

## Artifacts
Supported artifacts for Windows 7+ systems:

- [System Active Directory](https://forensics.wiki/active_directory/)
- [System Registry Hives](https://forensics.wiki/windows_registry/)
- [System Prefetch Files](https://forensics.wiki/prefetch/)
- [System Event Logs](https://forensics.wiki/windows_event_log_%28evt%29/)
- [System AmCache](https://forensics.wiki/amcache/)
- [User Registry Hives](https://forensics.wiki/windows_registry/)
- [User Jump Lists](https://forensics.wiki/jump_lists/)
- [User Browser Histories](https://forensics.wiki/google_chrome/)

## License
Released under the [MIT License](LICENSE.md).