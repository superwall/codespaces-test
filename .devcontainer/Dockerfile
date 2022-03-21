FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:0-16
RUN sudo apt-get update && \
	sudo apt-get install -y default-mysql-client && \
	sudo apt-get install -y apt-transport-https ca-certificates dirmngr && \
	sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 8919F6BD2B48D754 && \
	echo "deb https://packages.clickhouse.com/deb stable main" | sudo tee /etc/apt/sources.list.d/clickhouse.list && \
	sudo apt-get update && \
	sudo apt-get install -y clickhouse-client
