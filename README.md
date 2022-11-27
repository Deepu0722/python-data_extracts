# python-data_extracts
PDF  data extraction program using PyPDF2.PdfFileReader
**************************************************
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Install the latest PowerShell for new features and improvements! https://aka.ms/PSWindows

PS C:\Users\deepu\Desktop\deepu\python>  pip install PyPDF2 
Traceback (most recent call last):
  File "C:\Python310\lib\runpy.py", line 196, in _run_module_as_main
    return _run_code(code, main_globals, None,
  File "C:\Python310\lib\runpy.py", line 86, in _run_code
    exec(code, run_globals)
  File "C:\Python310\Scripts\pip.exe\__main__.py", line 4, in <module>
ModuleNotFoundError: No module named 'pip'
PS C:\Users\deepu\Desktop\deepu\python> pip install PyPDF2  
Traceback (most recent call last):
  File "C:\Python310\lib\runpy.py", line 196, in _run_module_as_main
    return _run_code(code, main_globals, None,
  File "C:\Python310\lib\runpy.py", line 86, in _run_code
    exec(code, run_globals)
  File "C:\Python310\Scripts\pip.exe\__main__.py", line 4, in <module>
ModuleNotFoundError: No module named 'pip'
PS C:\Users\deepu\Desktop\deepu\python> py -m pip --version
>>
C:\Python310\python.exe: No module named pip
PS C:\Users\deepu\Desktop\deepu\python> py -m ensurepip --default-pip
WARNING: Ignoring invalid distribution -ip (c:\python310\lib\site-packages)
WARNING: Ignoring invalid distribution -ip (c:\python310\lib\site-packages)
Looking in links: c:\Users\deepu\AppData\Local\Temp\tmp_wa8oc92
Requirement already satisfied: setuptools in c:\python310\lib\site-packages (63.2.0)
Processing c:\users\deepu\appdata\local\temp\tmp_wa8oc92\pip-22.2.1-py3-none-any.whl
WARNING: Ignoring invalid distribution -ip (c:\python310\lib\site-packages)
Installing collected packages: pip
  WARNING: Failed to write executable - trying to use .deleteme logic
ERROR: Could not install packages due to an OSError: [WinError 5] Access is denied: 'C:\\Python310\\Scripts\\pip.exe' -> 'C:\\Python310\\Scripts\\pip.exe.deleteme'   
Consider using the `--user` option or check the permissions.

Traceback (most recent call last):
  File "C:\Python310\lib\runpy.py", line 196, in _run_module_as_main
    return _run_code(code, main_globals, None,
  File "C:\Python310\lib\runpy.py", line 86, in _run_code
    exec(code, run_globals)
  File "C:\Python310\lib\ensurepip\__main__.py", line 5, in <module>
    sys.exit(ensurepip._main())
  File "C:\Python310\lib\ensurepip\__init__.py", line 287, in _main
    return _bootstrap(
  File "C:\Python310\lib\ensurepip\__init__.py", line 203, in _bootstrap
    return _run_pip([*args, *_PACKAGE_NAMES], additional_paths)
  File "C:\Python310\lib\ensurepip\__init__.py", line 104, in _run_pip
    return subprocess.run(cmd, check=True).returncode
  File "C:\Python310\lib\subprocess.py", line 524, in run
    raise CalledProcessError(retcode, process.args,
subprocess.CalledProcessError: Command '['C:\\Python310\\python.exe', '-W', 'ignore::DeprecationWarning', '-c', '\nimport runpy\nimport sys\nsys.path = [\'C:\\\\Users\\\\deepu\\\\AppData\\\\Local\\\\Temp\\\\tmp_wa8oc92\\\\setuptools-63.2.0-py3-none-any.whl\', \'C:\\\\Users\\\\deepu\\\\AppData\\\\Local\\\\Temp\\\\tmp_wa8oc92\\\\pip-22.2.1-py3-none-any.whl\'] + sys.path\nsys.argv[1:] = [\'install\', \'--no-cache-dir\', \'--no-index\', \'--find-links\', \'C:\\\\Users\\\\deepu\\\\AppData\\\\Local\\\\Temp\\\\tmp_wa8oc92\', \'setuptools\', \'pip\']\nrunpy.run_module("pip", run_name="__main__", alter_sys=True)\n']' returned non-zero exit status 1.
PS C:\Users\deepu\Desktop\deepu\python> python -m pip

Usage:
  C:\Python310\python.exe -m pip <command> [options]

Commands:
  install                     Install packages.
  download                    Download packages.
  uninstall                   Uninstall packages.
  freeze                      Output installed packages in requirements format.    
  inspect                     Inspect the python environment.
  list                        List installed packages.
  show                        Show information about installed packages.
  check                       Verify installed packages have compatible dependencies.
  config                      Manage local and global configuration.
  search                      Search PyPI for packages.
  cache                       Inspect and manage pip's wheel cache.
  index                       Inspect information available from package indexes.  
  wheel                       Build wheels from your requirements.
  hash                        Compute hashes of package archives.
  completion                  A helper command used for command completion.        
  debug                       Show information useful for debugging.
  help                        Show help for commands.

General Options:
  -h, --help                  Show help.
  --debug                     Let unhandled exceptions propagate outside the main  
                              subroutine, instead of logging them to stderr.       
  --isolated                  Run pip in an isolated mode, ignoring environment    
                              variables and user configuration.
  --require-virtualenv        Allow pip to only run in a virtual environment;      
                              exit with an error otherwise.
  -v, --verbose               Give more output. Option is additive, and can be     
                              used up to 3 times.
  -V, --version               Show version and exit.
  -q, --quiet                 Give less output. Option is additive, and can be     
                              used up to 3 times (corresponding to WARNING,        
                              ERROR, and CRITICAL logging levels).
  --log <path>                Path to a verbose appending log.
  --no-input                  Disable prompting for input.
  --proxy <proxy>             Specify a proxy in the form
                              scheme://[user:passwd@]proxy.server:port.
  --retries <retries>         Maximum number of retries each connection should     
                              attempt (default 5 times).
  --timeout <sec>             Set the socket timeout (default 15 seconds).
  --exists-action <action>    Default action when a path already exists:
                              (s)witch, (i)gnore, (w)ipe, (b)ackup, (a)bort.       
  --trusted-host <hostname>   Mark this host or host:port pair as trusted, even    
                              though it does not have valid or any HTTPS.
  --cert <path>               Path to PEM-encoded CA certificate bundle. If        
                              provided, overrides the default. See 'SSL
                              Certificate Verification' in pip documentation for   
                              more information.
  --client-cert <path>        Path to SSL client certificate, a single file        
                              containing the private key and the certificate in    
                              PEM format.
  --cache-dir <dir>           Store the cache data in <dir>.
  --no-cache-dir              Disable the cache.
  --disable-pip-version-check
                              Don't periodically check PyPI to determine whether   
                              a new version of pip is available for download.      
                              Implied with --no-index.
  --no-color                  Suppress colored output.
  --no-python-version-warning
                              Silence deprecation warnings for upcoming
                              unsupported Pythons.
  --use-feature <feature>     Enable new functionality, that may be backward       
                              incompatible.
  --use-deprecated <feature>  Enable deprecated functionality, that will be        
                              removed in the future.
PS C:\Users\deepu\Desktop\deepu\python> py -m pip install --upgrade pip setuptools wheel
WARNING: Ignoring invalid distribution -ip (c:\python310\lib\site-packages)
WARNING: Ignoring invalid distribution -ip (c:\python310\lib\site-packages)
Requirement already satisfied: pip in c:\python310\lib\site-packages (22.2.1)
Collecting pip
  Using cached pip-22.3.1-py3-none-any.whl (2.1 MB)
Requirement already satisfied: setuptools in c:\python310\lib\site-packages (63.2.0)
Collecting setuptools
  Downloading setuptools-65.6.3-py3-none-any.whl (1.2 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 1.2/1.2 MB 6.5 MB/s eta 0:00:00      

WARNING: Ignoring invalid distribution -ip (c:\python310\lib\site-packages)
WARNING: Ignoring invalid distribution -ip (c:\python310\lib\site-packages)
WARNING: Ignoring invalid distribution -ip (c:\python310\lib\site-packages)
PS C:\Users\deepu\Desktop\deepu\python> py -m venv tutorial_env
***************************************************
Install virtual environment & power shell then Pip install PyPDF2
PowerShell Extension v2022.11.0
Copyright (c) Microsoft Corporation.

https://aka.ms/vscode-powershell
Type 'help' to get help.

(tutorial_env) PS C:\Users\deepu\Desktop\deepu\python> pip install PyPDF2
Collecting PyPDF2
  Using cached pypdf2-2.11.2-py3-none-any.whl (220 kB)
Installing collected packages: PyPDF2
Successfully installed PyPDF2-2.11.2

[notice] A new release of pip available: 22.2.1 -> 22.3.1
[notice] To update, run: python.exe -m pip install --upgrade pip
(tutorial_env) PS C:\Users\deepu\Desktop\deepu\python> python ch1.py
Adobe Acrobat PDF Files
Adobe® Portable Document Format (PDF) is a universal file format that preserves all
of the fonts, formatting, colours and graphics of any source document, regardless ofthe application and platform used to create it.
Adobe PDF is an ideal format for electronic document distribution as it overcomes the
problems commonly encountered with electronic file sharing.
• Anyone, anywhere  can open a PDF file. All you need is the free Adobe Acrobat
Reader. Recipients of other file formats sometimes can't open files because they
don't have the applications used to create the documents.
• PDF files always print correctly  on any printing device.
• PDF files always display exactly  as created, regardless of fonts, software, and
operating systems. Fonts, and graphics are not lost due to platform, software, and
version incompatibilities.
• The free Acrobat Reader is easy to download and can be freely distributed by
anyone.
• Compact PDF files are smaller than their source files and download a
page at a time for fast display on the Web.
