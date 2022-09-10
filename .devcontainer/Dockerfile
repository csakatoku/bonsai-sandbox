FROM ocaml/opam:debian-11-ocaml-4.12

USER root
RUN apt install -y git pkg-config libssl-dev libffi-dev zlib1g-dev libgmp-dev libpcre3-dev

USER opam
RUN opam update

RUN opam install dune base merlin ocamlformat ppx_jane ocaml-lsp-server bonsai
