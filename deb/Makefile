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
	cd openresty-zlib; debclean
	find openresty-zlib -maxdepth 1 ! -name 'debian' ! -name 'openresty-zlib' -print | xargs rm -rf

download-openssl:
	wget 'https://www.openssl.org/source/old/1.0.2/openssl-1.0.2j.tar.gz'
	ln -s openssl-1.0.2j.tar.gz openresty-openssl_1.0.2j.orig.tar.gz

build-openssl:
	tar xf openresty-openssl_1.0.2j.orig.tar.gz --strip-components=1 -C openresty-openssl
	cd openresty-openssl; debuild

clean-openssl:
	cd openresty-openssl; debclean
	find openresty-openssl -maxdepth 1 ! -name 'debian' ! -name 'openresty-openssl' -print | xargs rm -rf

download-pcre:
	wget 'https://ftp.pcre.org/pub/pcre/pcre-8.39.tar.bz2'
	ln -s pcre-8.39.tar.bz2 openresty-pcre_8.39.orig.tar.bz2

build-pcre:
	tar xf openresty-pcre_8.39.orig.tar.bz2 --strip-components=1 -C openresty-pcre
	cd openresty-pcre; debuild

clean-pcre:
	cd openresty-pcre; debclean
	find openresty-pcre -maxdepth 1 ! -name 'debian' ! -name 'openresty-pcre' -print | xargs rm -rf

download-openresty:
	wget 'https://openresty.org/download/openresty-1.11.2.2.tar.gz'
	ln -s openresty-1.11.2.2.tar.gz openresty_1.11.2.2.orig.tar.gz

build-openresty:
	tar xf openresty_1.11.2.2.orig.tar.gz --strip-components=1 -C openresty
	cd openresty; debuild

clean-openresty:
	cd openresty; debclean
	find openresty -maxdepth 1 ! -name 'debian' ! -name 'openresty' -print | xargs rm -rf


### Makefile ends here
