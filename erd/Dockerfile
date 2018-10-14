FROM ubuntu:16.04

RUN apt-get update && \ 
    apt-get install -y software-properties-common  && \
    add-apt-repository -y ppa:hvr/ghc && \
    apt-get update && \
    apt-get install -y cabal-install ghc graphviz && \
    cabal update && \
    cabal install erd --allow-newer --global 

ENTRYPOINT [ "erd" ]