```
jaro@trr127hn01:~$ dpkg -l | grep "modules"
ii  apache2-bin                                      2.4.61-1~deb12u1                             amd64        Apache HTTP Server (modules and other binary files)
ii  cmake-data                                       3.25.1-1                                     all          CMake data files (modules, templates and documentation)
ii  glib-networking:amd64                            2.74.0-4                                     amd64        network-related giomodules for GLib
ii  glib-networking-common                           2.74.0-4                                     all          network-related giomodules for GLib - data files
ii  glib-networking-services                         2.74.0-4                                     amd64        network-related giomodules for GLib - D-Bus services
ii  grub-efi-amd64-bin                               2.06-13+deb12u1                              amd64        GRand Unified Bootloader, version 2 (EFI-AMD64 modules)
ii  kmod                                             30+20221128-1                                amd64        tools for managing Linux kernel modules
ii  libapache2-reload-perl                           0.13-4                                       all          module for reloading Perl modules when changed on disk
ii  libbio-cluster-perl                              1.7.3-6                                      all          BioPerl cluster modules
ii  libbio-perl-perl                                 1.7.8-1                                      all          BioPerl core perl modules
ii  libbio-perl-run-perl                             1.7.3-9                                      all          BioPerl wrappers: modules
ii  libclass-load-perl                               0.25-2                                       all          module for loading modules by name
ii  libdpkg-perl                                     1.21.22                                      all          Dpkg perl modules
ii  libextutils-f77-perl                             1.26-1                                       all          module to compile and link FORTRAN 77 code for Perl modules
ii  libgail-common:amd64                             2.24.33-2                                    amd64        GNOME Accessibility Implementation Library -- common modules
ii  libgl1-mesa-dri:amd64                            22.3.6-1+deb12u1                             amd64        free implementation of the OpenGL API -- DRI modules
ii  libhtml-parser-perl:amd64                        3.81-1                                       amd64        collection of modules that parse HTML text documents
ii  libio-sessiondata-perl                           1.03-3                                       all          set of modules for non-blocking I/O
ii  libio-stringy-perl                               2.111-3                                      all          modules for I/O on in-core objects (strings/arrays)
ii  libmailtools-perl                                2.21-2                                       all          modules to manipulate email in perl programs
ii  libmime-tools-perl                               5.510-1                                      all          Perl5 modules for MIME-compliant messages
ii  libp11-kit0:amd64                                0.24.1-2                                     amd64        library for loading and coordinating access to PKCS#11 modules - runtime
ii  libpam-modules:amd64                             1.5.2-6+deb12u1                              amd64        Pluggable Authentication Modules for PAM
ii  libpam-modules-bin                               1.5.2-6+deb12u1                              amd64        Pluggable Authentication Modules for PAM - helper binaries
ii  libparse-yapp-perl                               1.21-3                                       all          Perl module for creating fully reentrant LALR parser OO Perl modules
ii  libsasl2-modules:amd64                           2.1.28+dfsg-10                               amd64        Cyrus SASL - pluggable authentication modules
ii  libsasl2-modules-db:amd64                        2.1.28+dfsg-10                               amd64        Cyrus SASL - pluggable authentication modules (DB)
ii  libsub-quote-perl                                2.006008-1                                   all          helper modules for subroutines
ii  libsuitesparseconfig5:amd64                      1:5.12.0+dfsg-2                              amd64        configuration routines for all SuiteSparse modules
ii  libtimedate-perl                                 2.3300-2                                     all          collection of modules to manipulate date/time information
ii  libxml-perl                                      0.08-4                                       all          Perl modules for working with XML
ii  lmod                                             8.6.19-1                                     amd64        Lua based environment modules
ii  node-builtins                                    5.0.1-1                                      all          lists nodejs builtin modules
ii  node-cjs-module-lexer                            1.2.2+dfsg-5                                 all          Fast lexer to extract named exports from CommonJS modules
ii  node-es-module-lexer                             1.1.0+dfsg-2                                 all          Fast lexer to extract named exports from EcmaScript modules
ii  node-jest-debbundle                              29.3.1~ds1+~cs70.48.25-2                     all          various ittle Node.js modules needed by jest
ii  node-postcss-modules-extract-imports             3.0.0-2                                      all          CSS Modules transform to extract local aliases for inline imports
ii  node-postcss-modules-values                      4.0.0+~4.0.0-1                               all          pass arbitrary values between your module files
ii  node-v8-compile-cache                            2.3.0-3+deb12u1                              all          Leverage v8 compile cache to speedup loading of Node.js modules
ii  nvidia-modprobe                                  535.161.07-1~deb12u1                         amd64        utility to load NVIDIA kernel modules and create device nodes
ii  perl-modules-5.36                                5.36.0-7+deb12u1                             all          Core Perl modules
ii  python3-debian                                   0.1.49                                       all          Python 3 modules to work with Debian-related data formats
ii  python3-defusedxml                               0.7.1-2                                      all          XML bomb protection for Python stdlib modules (for Python 3)
ii  python3-pyasn1-modules                           0.2.8-1                                      all          Collection of protocols modules written in ASN.1 language (Python 3)
ii  python3-reportbug                                12.0.0                                       all          Python modules for interacting with bug tracking systems
ii  python3-sklearn                                  1.2.1+dfsg-1                                 all          Python modules for machine learning and data mining - Python 3
ii  r-cran-reticulate                                1.28+dfsg-1                                  amd64        R interface to Python modules, classes, and functions
ii  ruby-dev:amd64                                   1:3.1                                        amd64        Header files for compiling extension modules for Ruby (default version)
ii  ruby3.1-dev:amd64                                3.1.2-7+deb12u1                              amd64        Header files for compiling extension modules for the Ruby 3.1
ii  singular-modules:amd64                           1:4.3.1-p3+ds-2                              amd64        Computer Algebra System for Polynomial Computations -- module package
ii  webpack                                          5.75.0+dfsg+~cs17.16.14-1+deb12u1            all          Packs CommonJs/AMD modules for the browser
ii  zfs-dkms                                         2.1.11-1                                     all          OpenZFS filesystem kernel modules for Linux
jaro@trr127hn01:~$ conda --version
bash: conda: Kommando nicht gefunden.
jaro@trr127hn01:~$ dpkg -l | grep "conda"
ii  infernal                                         1.1.4-1                                      amd64        inference of RNA secondary structural alignments
ii  ncoils                                           2002-9                                       amd64        coiled coil secondary structure prediction
jaro@trr127hn01:~$
```