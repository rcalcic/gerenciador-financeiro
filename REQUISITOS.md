# Requisitos do Gerenciador Financeiro

## Para usar o app

| Item | Requisito |
| --- | --- |
| Sistema | Windows 10 de 64 bits (versão 1809 ou mais nova) ou Windows 11 |
| Navegador | Microsoft Edge (já vem no Windows) ou Google Chrome — abre a janela do app e gera os PDFs |
| Memória | 4 GB |
| Disco | 200 MB livres para o programa, mais o espaço dos backups (alguns MB) |
| Permissão | Conta de usuário comum: a instalação não pede administrador |
| Internet | Só para buscar atualizações (opcional) |

O instalador confere o Windows, os 64 bits e o navegador antes de instalar.

## Por recurso (opcionais)

| Recurso | O que precisa |
| --- | --- |
| Backup na nuvem | Uma pasta sincronizada (OneDrive, Google Drive para computador ou Dropbox) escolhida como pasta dos backups |
| Avisos de vencimento | Notificações do Windows ligadas para o app |
| Relatórios em PDF | Microsoft Edge ou Google Chrome instalado |
| Windows Hello | PIN, digital ou rosto configurados em Configurações › Contas › Opções de entrada (TPM 2.0 recomendado) |
| Celular | Celular e computador na **mesma rede** (não na rede de convidados), Chrome no Android ou Safari no iPhone, rede do Windows como **privada** ou a liberação do firewall (o botão "Liberar no firewall" pede administrador uma vez), roteador sem "isolamento de dispositivos", computador ligado com o app aberto ou na bandeja |
| IA local | [Ollama](https://ollama.com/download) instalado e aberto; 8 GB de memória para o modelo leve (qwen2.5:3b, 1,9 GB) ou 16 GB para o recomendado (qwen2.5:7b, 4,7 GB); placa de vídeo opcional (deixa as respostas mais rápidas) |
| Telegram | Conta no Telegram, um bot criado no @BotFather, internet no computador, computador ligado com o app desbloqueado (pode ficar na bandeja) |

## Antivírus e EDR

O programa ainda não tem assinatura de código (certificado de editor). Em computadores com política de segurança
corporativa (EDR), pode ser preciso liberar `GerenciadorFinanceiro.exe` e `Instalar-GerenciadorFinanceiro.exe`.
As versões publicadas são conferidas por SHA-256 e assinatura Ed25519 antes de cada atualização automática.
