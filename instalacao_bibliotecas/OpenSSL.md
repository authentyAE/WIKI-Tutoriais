# Compilando e Instalando OpenSSL

OpenSSL é uma biblioteca completa e bastante avançada para criptografia e cálculo de cógigos Hash, para C++.
O passo a passo completo pode ser visto abaixo:
[Windows Notes](https://github.com/openssl/openssl/blob/master/NOTES-WINDOWS.md) e [Build and Install](https://github.com/openssl/openssl/blob/master/INSTALL.md)

## Pré-Requisitos
- Visual Studio 2019 com:
  - Desenvolvimento para desktop com C++;
  - Desenvolvimento para desktop com .NET (Opcional);
  - Desenvolvimento com a Plataforma Universal do Windows (Opcional);
  - **Desenvolvimento para Linux com C++**
- Instalar (ou extrair) Perl, e adiciona-lo ao PATH do sistema (`...\perl\bin\`);
  - Download: [Site Oficial](http://strawberryperl.com/)
- Instalar (ou extrair) NASM, e adiciona-lo ao PATH do sistema;
  - Download: [Site Oficial](https://www.nasm.us/)

## Compilação
- Abrir pasta do OpenSSL no Visual Studio 2019 (**COM PRIVILÉGIOS DE ADMINISTRADOR**)
  - Download: [OpenSSL - Repositório GitHub](https://github.com/openssl/openssl.git)
- Abrir terminal do compilador:
  - Terminal -> Novo Terminal
- Executar ferramenta VCVARSALL, compilar e instalar, para 32bits **(Tempo Necessário: Mais de 30min)**
  - > `C:\"Program Files (x86)"\"Microsoft Visual Studio"\2019\Professional\VC\Auxiliary\Build\vcvarsall.bat x86`
  - > `perl Configure VC-WIN32`
  - > `nmake`
  - > `nmake test`
  - > `nmake install`
  - COMANDO COMPLETO: `C:\"Program Files (x86)"\"Microsoft Visual Studio"\2019\Professional\VC\Auxiliary\Build\vcvarsall.bat x86 && perl Configure VC-WIN32 && nmake && nmake test && nmake install`
