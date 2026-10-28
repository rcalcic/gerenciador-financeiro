# Notas de versão

## 1.0.2 — 29/10/2026

### Correções
- Celular: depois de atualizar o app, aparecia "a porta 47614 está ocupada" mesmo com o acesso funcionando. A versão anterior agora libera a porta antes de a nova abrir, o app tenta de novo por alguns segundos e o aviso some quando o acesso liga.

## 1.0.1 — 29/10/2026

### Correções
- Celular: a página não abria no Chrome do Android (erro ERR_TOO_MANY_RETRIES). A conexão agora é cifrada pelo próprio app, sem certificado: abre direto no Chrome e no Safari, sem o aviso de "conexão não particular".
- Atualização: o antivírus do Windows bloqueava o programa baixado. O programa deixou de ser ofuscado e, se o antivírus barrar uma atualização, o app avisa onde conferir.

### Melhorias
- Código de conexão do celular com 16 letras e números; pelo QR Code a conexão continua automática e a chave não passa pela rede.

## 1.0.0 — 29/10/2026

### Novidades
- Contas do mês com categorias, pagamento, tipo (recorrente, parcelada ou avulsa), dia de vencimento e perfil; copiar do mês anterior, importar planilha do Excel e exportar CSV.
- Importação de faturas de cartão, contas de consumo, holerites e férias por PDF ou foto (OCR), com calibração da leitura por emissor.
- Parcelamentos aprendidos das faturas e lançados em todos os meses até quitar, sem duplicar ao importar a fatura seguinte.
- Entradas e Rendimentos: Pagamento CLT (holerites, descontos, projeção do salário com adiantamento e saldo), Avulsos e FGTS.
- Calendário de pagamentos, com avisos no Windows antes do vencimento, mesmo com o app fechado.
- Metas e reserva de emergência, com progresso e ritmo necessário por mês.
- Orçamento por categoria, com alerta em 80% e ao estourar.
- Simulador "e se…": antecipar parcelamento, nova compra parcelada, mudança de salário e despesas mensais ou únicas.
- Imposto de Renda: resumo do ano-calendário com exportação em PDF.
- Patrimônio: investimentos, bens e dívidas, com evolução do patrimônio líquido.
- Gastos do cartão com categorias automáticas que aprendem com as correções.
- Assinaturas: custo mensal e anual e aviso de mudança de preço.
- Perfis para separar as contas de cada pessoa ou casa, com o consolidado.
- Uso pelo celular na rede Wi-Fi de casa, sem internet: QR Code que já conecta o aparelho, no Chrome (Android) ou no Safari (iPhone), com atalho na tela de início.
- Opção de manter o app em execução na bandeja do sistema ao fechar a janela, e de iniciar com o Windows na bandeja: o celular funciona com o computador ligado e pede a senha do app para desbloquear.
- Início com alertas, nota de saúde financeira e resumo do mês; Evolução anual, Consumo, Gráficos e relatórios em PDF.
- Meu Consultor Pessoal: respostas e dicas calculadas com os seus dados, sem enviar nada para a internet.
- Backups: os 4 últimos para restaurar, restauração de um arquivo de qualquer pasta e troca da pasta dos backups pelo app.
- Aviso de atualização com as notas da versão e a escolha de atualizar agora ou depois.
- Quem usa o Finanças Pessoais 2.x ou 3.0 recebe esta versão pelo "Verificar atualização" (ou pelo instalador), mantendo senha, dados e backups; programa, atalhos e registro passam a se chamar Gerenciador Financeiro.

### Segurança
- Banco de dados e backups cifrados com AES-256-GCM, abertos só com a senha ou com o código de recuperação.
- Backup automático a cada fechamento.
- Atualização automática com verificação de assinatura digital.
- Programa publicado com a interface cifrada dentro do executável.
