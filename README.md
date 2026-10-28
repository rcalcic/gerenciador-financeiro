# Gerenciador Financeiro

**Calcic SoftwareHouse** · criado por **Rodrigo Calcic** · freeware para Windows 10 e 11

Controle financeiro pessoal completo e privado: contas do mês, faturas de cartão e holerites lidos
direto do PDF, parcelamentos, calendário de pagamentos, metas, orçamento, simulador, Imposto de Renda,
patrimônio e uso pelo celular na rede de casa. Os dados ficam **só no seu computador**, cifrados.

## ⬇️ Baixar

**[Instalar-GerenciadorFinanceiro.exe — versão mais recente](https://github.com/rcalcic/gerenciador-financeiro/releases/latest/download/Instalar-GerenciadorFinanceiro.exe)**

[Notas de versão](CHANGELOG.md) · [Todas as versões](https://github.com/rcalcic/gerenciador-financeiro/releases)

1. Rode o instalador (não precisa de administrador).
2. Escolha a pasta do programa e a pasta dos backups (de preferência no OneDrive).
3. Na primeira abertura, crie a senha e guarde o código de recuperação.

Já usa a versão anterior (**Finanças Pessoais**)? Use **Verificar atualização** no próprio app (ou rode o
instalador novo): o programa é trocado e a senha, os dados e os backups continuam. A Release
"Finanças Pessoais → Gerenciador Financeiro" existe só para essas versões antigas encontrarem a atualização. Depois disso o app se atualiza sozinho: ao abrir, ele avisa quando há
versão nova, mostra o que mudou e pergunta se você quer atualizar.

## Telas

> Imagens com **dados fictícios de demonstração**.

| Início | Mês |
| --- | --- |
| ![Início](docs/telas/00-inicio.png) | ![Mês](docs/telas/01-mes.png) |
| **Calendário de pagamentos** | **Metas** |
| ![Calendário](docs/telas/16-calendario.png) | ![Metas](docs/telas/17-metas.png) |
| **Orçamento por categoria** | **Simulador "e se…"** |
| ![Orçamento](docs/telas/25-orcamento.png) | ![Simulador](docs/telas/18-simulador.png) |
| **Gastos do cartão** | **Assinaturas** |
| ![Gastos do cartão](docs/telas/19-gastos-cartao.png) | ![Assinaturas](docs/telas/20-assinaturas.png) |
| **Patrimônio** | **Imposto de Renda** |
| ![Patrimônio](docs/telas/21-patrimonio.png) | ![Imposto de Renda](docs/telas/22-imposto-renda.png) |
| **Perfis** | **Pagamento CLT** |
| ![Perfis](docs/telas/24-perfis.png) | ![Pagamento CLT](docs/telas/12-entradas-descontos.png) |
| **Parcelamentos** | **Evolução anual** |
| ![Parcelamentos](docs/telas/05-parcelamentos.png) | ![Evolução anual](docs/telas/04-evolucao.png) |
| **Gráficos** | **Meu Consultor Pessoal** |
| ![Gráficos](docs/telas/02-graficos.png) | ![Meu Consultor Pessoal](docs/telas/06-consultor.png) |
| **Celular: conectar pelo QR Code** | **Celular (Chrome ou Safari)** |
| ![Conectar o celular](docs/telas/23-celular-computador.png) | ![Celular](docs/telas/23-celular.png) |
| **Backups** | **Aviso de atualização** |
| ![Backups](docs/telas/26-backups.png) | ![Atualização](docs/telas/27-atualizacao.png) |
| **Tema escuro** | **Tela de senha** |
| ![Tema escuro](docs/telas/09-tema-escuro.png) | ![Senha](docs/telas/10-senha.png) |

## Recursos

- **Contas do mês**: categorias, pago/a pagar, recorrentes e parceladas, dia de vencimento, perfis, copiar do mês anterior, planilha do Excel e CSV.
- **Importação por PDF ou foto** (OCR no próprio computador): faturas de cartão, contas de consumo, holerites e férias.
- **Parcelamentos** aprendidos das faturas e lançados em todos os meses até quitar.
- **Entradas e Rendimentos**: Pagamento CLT (adiantamento e saldo), Avulsos e FGTS.
- **Calendário de pagamentos** com avisos do Windows antes do vencimento, mesmo com o app fechado.
- **Metas**, **Orçamento**, **Simulador "e se…"**, **Imposto de Renda** (com PDF), **Patrimônio**, **Assinaturas**, **Perfis**.
- **Meu Consultor Pessoal**: respostas e dicas calculadas com os seus números, sem enviar nada para a internet.
- **Celular**: abra pelo QR Code no Chrome (Android) ou no Safari (iPhone), na rede Wi-Fi de casa.
- **Bandeja do sistema**: o app pode continuar rodando na bandeja ao fechar a janela e iniciar com o Windows; basta o computador estar ligado para o celular funcionar (ele pede a senha do app para desbloquear).

## Privacidade e segurança

- Banco de dados e backups cifrados com **AES-256-GCM**; só abrem com a senha ou com o código de recuperação.
- Nada vai para a internet: o app só consulta este repositório para saber se há versão nova.
- Atualizações conferidas por **assinatura digital** (Ed25519) e SHA-256 antes de instalar; backup antes de trocar o programa.
- Celular: desligado por padrão, só na rede local, conversa cifrada pelo próprio app (ChaCha20 + HMAC-SHA256) e pareamento pelo QR Code.
- Backup a cada fechamento: os 4 últimos ficam disponíveis, dá para restaurar de qualquer arquivo e trocar a pasta dos backups.
- Código-fonte fechado: neste repositório ele fica apenas cifrado, usado pelo GitHub Actions para compilar, testar e assinar cada versão.
