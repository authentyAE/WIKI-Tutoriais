# Compilando e Instalando OpenSSL

OpenSSL é uma biblioteca completa e bastante avançada para criptografia e cálculo de cógigos Hash, para C++.

## Pré-Requisitos
- Visual Studio 2019 com:
  - Desenvolvimento para desktop com C++;
  - Desenvolvimento para desktop com .NET (Opcional);
  - Desenvolvimento com a Plataforma Universal do Windows (Opcional);
  - **Desenvolvimento para Linux com C++**
- Instalar (ou extrair) Perl
  - Download: [Site Oficial](http://strawberryperl.com/)
- Instalar (ou extrair) NASM
  - Download: [Site Oficial](https://www.nasm.us/)

## Compilação
- Abrir pasta do OpenSSL no Visual Studio Code
  - Download: [OpenSSL - Repositório GitHub](https://github.com/openssl/openssl.git)
- Abrir terminal do compilador:
  - Terminal -> Novo Terminal
- Executar ferramenta VCVARSALL para 32bits **(Tempo: Compilação= 15min + Teste = 10min + Instalação = 15min)**
  - > C:\"Program Files (x86)"\"Microsoft Visual Studio"\2019\Professional\VC\Auxiliary\Build\vcvarsall.bat x86
  - > perl Configure VC-WIN32
  - > nmake
  - > nmake test
  - > nmake install
