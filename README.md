# WebVM

A fork of [WebVM](https://github.com/leaningtech/webvm) that is designed to be a web-based developer envoronment that runs entirely using WASM.

# Modifications to [upstream](https://github.com/leaningtech/webvm)

- Use alpine linux instead of debian since it has better packages in the repos
- Remove some packages that I wouildn't use like nodejs and ruby
- Install some packages that I would use like helix, nushell, and lf
- Clone the [common-assembly](https://github.com/godalming123/common-assembly) codebase into the home directory
- Update the default shell to nushell, and the default editor to helix

# Thanks to...

This project depends on:

- [CheerpX](https://cheerpx.io/), made by [Leaning Technologies](https://leaningtech.com/) for x86 virtualization and Linux emulation
- xterm.js, [https://xtermjs.org/](https://xtermjs.org/), for providing the Web-based terminal emulator
- [Tailscale](https://tailscale.com/), for the networking component
- [lwIP](https://savannah.nongnu.org/projects/lwip/), for the TCP/IP stack, compiled for the Web via [Cheerp](https://github.com/leaningtech/cheerp-meta/)

# Versioning

WebVM depends on the CheerpX x86-to-WebAssembly virtualization technology, which is included in the project via [NPM](https://www.npmjs.com/package/@leaningtech/cheerpx).

The NPM package is updated on every release.

Every build is immutable, if a specific version works well for you today, it will keep working forever.

# License

WebVM is released under the Apache License, Version 2.0.

You are welcome to use, modify, and redistribute the contents of this repository.

The public CheerpX deployment is provided **as-is** and is **free to use** for technological exploration, testing and use by individuals. Any other use by organizations, including non-profit, academia and the public sector, requires a license. Downloading a CheerpX build for the purpose of hosting it elsewhere is not permitted without a commercial license.

Read more about [CheerpX licensing](https://cheerpx.io/docs/licensing)

If you want to build a product on top of CheerpX/WebVM, please get in touch: sales@leaningtech.com
