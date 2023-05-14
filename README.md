# Apache httpd mod_fcgid - Windows MSVC binaries #
forked from :  https://github.com/pagespeed/mod_fcgid

fixes : https://github.com/pagespeed/mod_fcgid/compare/master...nono303:mod_fcgid:master 

----
### Version [2.3.10.2](https://github.com/nono303/mod_fcgid/releases/tag/2.3.10.2)
> 2022-07-26 - commit
>
> 2023-05-14-16 - build

- **VS17** toolset: 14.36.32530
- **VS16** toolset: 14.29.30133
- **VC15** toolset: 14.16.27023
- MSVC redist:  [x86](https://aka.ms/vs/16/release/vc_redist.x86.exe) - [x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)
- Window Kit: 10.0.22621.0
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** _in specified directory_

|          | x86  | x64  |
| -------- | ---- | ---- |
| **VS17** | ❌    | ✅ |
| **VS16** | ❌    | ❌ |
| **VC15** | ❌    | ❌ |

> _just open an issue if you need a release not present_

**Build Scripts** 

- [@nono303/win-build-scripts](https://github.com/nono303/win-build-scripts)
  - cflags: `/O2 /GL /MD /Zi`
  - ldflags: ` /LTCG /OPT:REF,ICF`


**Build  & Runtime Dependencies**

> * All dependencies are built from sources in the same context
>
> * Check it with`dumpbin /DEPENDENTS mod_md.so`

- [apr 1.8.0-dev](https://github.com/apache/apr) - `libapr-1.dll`
- [apr-util 1.7.0-dev](https://github.com/apache/apr-util) - `libaprutil-1.dll`
- [httpd 2.4.57](https://github.com/apache/httpd/tree/2.4.57) - `libhttpd.dll`



