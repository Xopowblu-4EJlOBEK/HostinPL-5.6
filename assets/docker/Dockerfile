FROM debian:stretch
RUN echo "deb http://deb.debian.org/debian stretch main" > /etc/apt/sources.list \
	&& echo "deb-src http://deb.debian.org/debian stretch main" >> /etc/apt/sources.list \
	&& echo "deb http://security.debian.org/debian-security stretch/updates main" >> /etc/apt/sources.list \
	&& echo "deb-src http://security.debian.org/debian-security stretch/updates main" >> /etc/apt/sources.list \
	&& echo "deb http://deb.debian.org/debian stretch-updates main" >> /etc/apt/sources.list \
	&& echo "deb-src http://deb.debian.org/debian stretch-updates main" >> /etc/apt/sources.list
RUN dpkg --add-architecture i386
RUN apt-get update && apt-get install -y libstdc++6:i386 libgcc1:i386 zlib1g:i386 libncurses5:i386
RUN apt-get install -y libbabeltrace1 libc6-dbg libdw1 lib32stdc++6 libreadline5 gdb-minimal
RUN apt-get update && apt-get install -y gnupg screen apt-transport-https curl
RUN echo 'deb https://deb.nodesource.com/node_14.x stretch main' > /etc/apt/sources.list.d/nodesource.list \
	&& echo 'deb-src https://deb.nodesource.com/node_14.x stretch main' >> /etc/apt/sources.list.d/nodesource.list \
	&& curl -sLf -o /dev/null 'https://deb.nodesource.com/node_14.x/dists/stretch/Release' \ 
	&& curl -s https://deb.nodesource.com/gpgkey/nodesource.gpg.key | apt-key add - \
	&& curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add - \
	&& echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
RUN apt-get update
RUN apt-get install -y gcc g++ make nodejs yarn