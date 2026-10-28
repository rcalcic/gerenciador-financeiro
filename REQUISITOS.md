# Requisitos do Gerenciador Financeiro

## Para usar o app

| Item | Requisito |
| --- | --- |
| Sistema | Windows 10 de 64 bits (versão 1809 ou mais nova) ou Windows 11 |
| Navegador | Microsoft Edge (já vem no Windows) ou Google Chrome — abre a janela do app e gera os PDFs |
| Memória | 4 GB |
| Disco | 2 GB livres (programa e IA local embutida), mais o espaço dos backups (alguns MB) |
| Permissão | Conta de usuário comum: a instalação não pede administrador |
| Internet | Só para buscar atualizações (opcional) |

O instalador confere o Windows, os 64 bits e o navegador antes de instalar. Ele tem cerca de 1,2 GB porque traz a IA local; a cópia guardada na pasta dos backups é a versão leve, sem a IA.

## Por recurso (opcionais)

| Recurso | O que precisa |
| --- | --- |
| Backup na nuvem | Uma pasta sincronizada (OneDrive, Google Drive para computador ou Dropbox) escolhida como pasta dos backups |
| Avisos de vencimento | Notificações do Windows ligadas para o app |
| Dados do mercado | Internet. O programa consulta só a Selic e o IPCA no Banco Central (dados públicos); nenhuma informação do aplicativo é enviada |
| IA local | Já vem no instalador (modelo Leve, cerca de 1,1 GB) e é instalada e ligada automaticamente. Memória: 4 GB (8 GB recomendados; o modelo Melhor, baixado à parte, pede 8 GB). Funciona sem internet |
| Relatórios em PDF | Microsoft Edge ou Google Chrome instalado |

## Antivírus e EDR

O programa ainda não tem assinatura de código (certificado de editor). Em computadores com política de segurança
corporativa (EDR), pode ser preciso liberar `GerenciadorFinanceiro.exe` e `Instalar-GerenciadorFinanceiro.exe`.
As versões publicadas são conferidas por SHA-256 e assinatura Ed25519 antes de cada atualização automática.
