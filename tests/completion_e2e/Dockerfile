#FROM alpine:3.10
#RUN apk --no-cache add zsh=5.7.1-r0
#COPY complete-zsh.zsh git-machete.completion.zsh ./
#RUN zsh --version && zsh -x complete-zsh.zsh "git machete "

FROM ubuntu:22.04
RUN apt-get update
RUN apt-get install -y zsh
COPY complete-zsh.zsh git-machete.completion.zsh ./
RUN zsh --version && zsh complete-zsh.zsh "git machete "
