# Third-Party Components

This repository contains the source code and patches for the third-party
libraries:

* DiscUtils (v0.7) - a .NET library for reading and writing ISO files
  and Virtual Machine disk files (VHD, VDI, XVA, VMDK, etc);
* DotNetZip (v1.9.1.8) - a .NET library for handling ZIP files;
* SharpZipLib (v0.85.4)- a Zip, GZip, Tar and BZip2 library written
  entirely in C# for the .NET platform;
* XML-RPC.NET (v2.5.0) - a library for implementing XML-RPC Services
  and clients in the .NET environment;
* log4net (v1.2.13) - a library providing logging services for purposes
  of application debugging and auditing;
* Json.NET (v10.0.2) - a Json framework for .NET.

## Contributions

How to submit changes
=====================

Please try to follow the guidelines below. They will make things
easier on the maintainers. Not all of these guidelines matter for every
trivial change so apply some common sense.

If you are unsure about something written here, ask on the XCP-ng forum https://xcp-ng.org/forum/

0.    Before starting a big project, discuss it on the list first :-)

1.    Always test your changes, however small, by both targetted 
      manual testing and by running the unit tests.

2.	  When adding new functionality, include test cases for any 
	  * important; or 
	  * difficult to manually test; or 
	  * easy to break
	  new code.

3.    Make your patch(es) available by creating one or more github pull requests. 
      Each pull request should be separately reviewable and mergable. Only patches 
      which must be committed together should be in the same pull request.

4.    Each patch should include a descriptive commit comment that helps
      understand why the patch is necessary and why it works. This will
      be used both for initial review and for new people to understand
      how the code works later.

5.    For bonus points, ensure the project still builds in between every
      patch in a set: this helps hunt down future regressions with 'bisect'.

6.    Make sure you have the right to submit any changes you make. If you
      do changes at work you may find your employer owns the patches
      instead of you.

----------------------------------------------------------------------------
	  
For a list of maintainers, please see MAINTAINERS file.

## License

This code is licensed under the BSD 2-Clause license. The individual libraries
are subject to their own licenses, which can be found in the corresponding
directories. Please see the LICENSE file for more information.

## How to build dotnet-packages

The libraries can be built (and patches applied) by executing the script
`build.sh` at the command line (you'll need [Cygwin](http://www.cygwin.com)).
