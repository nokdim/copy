To use Copy in Linux, install this tarball wherever you like. There are three
binaries available for use, described below.

1.  CopyAgent – This is a QT based UI application for the Linux GUI; it acts
    as a tray application, just like the Mac and Windows versions.
1.a     You can install overlays on certain version of Nautilus, by
        running as root ./CopyAgent –installOverlay.

2.  CopyConsole – This is a headless version of the Copy app. It can run
    in a terminal or as a background process.
2.a     This version won't have a login prompt, so if you haven't logged
        in before you'll need to provide at minimum a username and Copy
        folder location. If a password isn't provided at the command line,
        it will be prompted for. Example:
        CopyConsole -username=<email> -root=/home/<user>/Copy
2.b     If you have previously logged in, either with CopyAgent or
        CopyConsole, then no special arguments are required.
2.c     For more options, run: CopyCommand -help

3.  CopyCmd – This is a tool that provides commandline APIs into various
    aspects of the Copy app. You can do cool things like create a link
    URL to a file in your account or upload a file directly into
    the cloud.
3.a     For a full list of commands, run: CopyCmd -help
3.b     Several commands require a [path] as an argument. All such paths
        must begin with / and are relative to your Copy folder. For
        example, if your Copy folder contains a subdirectory called Foo,
        and inside that is a file called Bar, then the [path] argument
        needed to refer to file Bar would be /Foo/Bar.
