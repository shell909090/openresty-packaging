### Makefile --- 

## Author: shell@xps13
## Version: $Id: Makefile,v 0.0 2017/03/22 04:56:03 shell Exp $
## Keywords: 
## X-URL: 


download-zlib:
	wget 'http://www.zlib.net/fossils/zlib-1.2.8.tar.gz'
	ln -s zlib-1.2.8.tar.gz openresty-zlib_1.2.8.dfsg.orig.tar.gz

build-zlib:
	tar xf openresty-zlib_1.2.8.dfsg.orig.tar.gz --strip-components=1 -C openresty-zlib
	cd openresty-zlib; debuild

clean-zlib:
	find openresty-zlib -maxdepth 1 ! -name 'debian' ! -name 'openresty-zlib' -print | xargs rm -rf
	cd openresty-zlib; debclean

### Makefile ends here
