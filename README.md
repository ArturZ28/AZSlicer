<div align="center">

<img alt="AZSlicer" src="resources/images/OrcaSlicer_horizontal_light.svg" width="320">

**AZSlicer** — fatiador FDM da **AZ3D Tecnologia**

</div>

## O que é

O AZSlicer é uma edição do [OrcaSlicer](https://github.com/OrcaSlicer/OrcaSlicer) personalizada pela AZ3D Tecnologia.
Ele tem as mesmas funções do OrcaSlicer, incluindo todos os perfis de impressoras, filamentos e processos
que vêm com ele (73 fabricantes e 455 modelos de impressora, entre eles a Snapmaker U1), com a marca, o ícone e
o nome da AZ3D.

## O que muda em relação ao OrcaSlicer

- Nome, ícone, logo, tela inicial, tela "Sobre" e textos da interface trocados para AZSlicer (todas as traduções, incluindo pt-BR).
- Pasta de configurações própria (`%APPDATA%\AZSlicer`): pode ser instalado no mesmo computador que o OrcaSlicer, sem misturar perfis.
- Instalador próprio (`AZSlicer_Windows_Installer_*.exe`), com atalho e entrada em "Programas instalados" como AZSlicer.
- O aviso automático de nova versão do OrcaSlicer foi desligado, para não oferecer o instalador do Orca aos usuários do AZSlicer.
- Arquivos de projeto (.3mf) e G-code continuam compatíveis com OrcaSlicer, Bambu Studio e impressoras Klipper/Moonraker.

## Como gerar o instalador para Windows

O instalador é gerado pelo GitHub Actions (workflow **AZSlicer Windows**):

1. Cada envio para a branch `main` gera o instalador e a versão portátil. Eles ficam em **Actions → execução → Artifacts**.
2. Para publicar uma versão, crie uma tag começando com `v` (por exemplo `v2.6.0-az1`). O instalador vai para a página **Releases**.
3. A primeira compilação leva de 2 a 3 horas, porque compila todas as dependências. As seguintes reaproveitam o cache.

## Licença

O AZSlicer é software livre, distribuído sob a **GNU Affero General Public License v3.0** (veja [LICENSE.txt](LICENSE.txt)),
a mesma licença do OrcaSlicer. Quem distribuir o programa deve disponibilizar o código-fonte correspondente.
Este repositório cumpre essa exigência.

Créditos: OrcaSlicer (SoftFever e colaboradores), baseado no Bambu Studio (Bambu Lab), que por sua vez é baseado no
PrusaSlicer (Prusa Research) e no Slic3r (Alessandro Ranellucci e a comunidade RepRap). O README original do projeto
está em [README_OrcaSlicer.md](README_OrcaSlicer.md).

"OrcaSlicer" é nome do projeto original. O AZSlicer não é um produto oficial do OrcaSlicer nem é endossado por ele.
