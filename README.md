# WhatsApp Disparador — Releases

Este repositório contém **apenas o instalador e os arquivos de atualização** do WhatsApp Disparador. O código-fonte fica no repositório privado.

## Download

Baixe o instalador mais recente em [Releases](https://github.com/BillHebertPDC/whatsapp-disparador-releases/releases/latest).

- Windows 10/11, 64 bits.
- Instalador NSIS com escolha de diretório.
- Atualizações automáticas pelo próprio aplicativo.

## Primeira instalação

1. Baixe WhatsApp-Disparador-0.1.0-x64.exe.
2. Execute o instalador.
3. Abra o aplicativo e configure a API key do WAHA e do Gemini em **Configurações**.

O instalador não possui assinatura de código nesta versão. O Windows SmartScreen pode exibir um aviso; use **Mais informações → Executar assim mesmo** apenas se o arquivo veio deste repositório.

## Verificação

Cada release inclui um arquivo .sha256. No PowerShell:

`powershell
Get-FileHash .\WhatsApp-Disparador-0.1.0-x64.exe -Algorithm SHA256
`

Compare o hash com o conteúdo do .sha256 publicado na release.

## Atualizações

O aplicativo verifica atualizações alguns segundos após abrir. O download é automático e a instalação é confirmada pelo botão **Reiniciar e instalar**. Se houver envios em andamento, a instalação é bloqueada até terminar.