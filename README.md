# MAGIC PLAYER

Sistema estático para criar páginas de reprodução compartilháveis e QR Codes.

## Publicação no GitHub Pages
1. Abra **Settings → Pages**.
2. Em **Build and deployment**, selecione **Deploy from a branch**.
3. Escolha a branch **main** e a pasta **/(root)**.
4. Salve. O endereço ficará em https://adoniasnascimento93-blip.github.io/magic-player/

## Como funciona
- Cada player guarda título, endereço de origem e capa opcional dentro do próprio link compartilhável.
- QR Code aponta para o link do player.
- MP4 direto é reproduzido em um elemento de vídeo HTML5.
- Google Drive e OneDrive usam tentativa de incorporação; permissões e políticas do provedor podem impedir a reprodução.
- Google Photos e links de páginas comuns não garantem incorporação. Prefira um link MP4 direto.
- Reprodução automática é solicitada sem som, pois navegadores móveis normalmente bloqueiam autoplay com áudio.

## Dados
A lista administrativa é armazenada no localStorage do navegador. Use Exportar JSON para backup e Importar JSON em outro dispositivo. O sistema ainda não possui banco de dados compartilhado nem autenticação multiusuário.

## QR Code
A imagem do QR é gerada pelo serviço externo QRServer; para uso offline ou privacidade adicional, substitua por uma biblioteca QR local.
