# Notas de versão

## 1.6.1 — 03/11/2026

### Melhorias
- Pagamento CLT: "Importar holerite ou férias" aceita vários arquivos de uma vez. Selecione o holerite do salário e o do adiantamento juntos: o app abre um por vez para conferir, mapeia proventos, descontos, FGTS e bases de cálculo, e a projeção e a evolução mês a mês passam a usar esses dados.

## 1.6.0 — 03/11/2026

### Novidades
- Botão "Detalhes" em cada conta do mês: mostra o resumo (valor, vencimento, referência, situação, consumo e custo por unidade, código de pagamento) e permite ajustar valor, vencimento, consumo, mês de referência e se está paga, sem precisar importar de novo. Também tem atalhos para importar a fatura e para o boleto/Pix.

### Melhorias
- Projeção de entradas: sem nenhum holerite mensal, o salário bruto passa a ser calculado pelo adiantamento importado (adiantamento ÷ percentual, 40% por padrão), e os descontos são aplicados pela tabela CLT. Antes, sem holerite, o mês ficava sem projeção.
- Leitura de fatura de cartão (calibrada com a fatura do Mercado Pago): o "Pagamento da fatura" anterior deixa de entrar como gasto; os itens somam exatamente o total.

### Correções
- Fatura do Mercado Pago: o pagamento da fatura anterior era lançado como item marcado e distorcia a soma.

## 1.5.0 — 03/11/2026

### Novidades
- Cada conta fica no mês em que é lançada e paga: o que você importa ou lança em Novembro vale para Novembro, mesmo sendo uma conta de outubro. O mês de referência impresso na conta (ex.: Outubro/2026) é guardado como base de consumo, então a tela Consumo continua mostrando Outubro. A importação não muda mais o mês pelo vencimento.
- Férias: ao marcar "Mês de férias" em Novembro, o desconto do salário é projetado para Dezembro (adiantamento do dia 20 de novembro e saldo de dezembro). Novembro mantém o salário de outubro integral e o recibo de férias.

### Melhorias
- O Calendário passa a datar o salário assim: o saldo no dia 5 do próprio mês e o adiantamento no dia 20 do mês anterior ao lançamento.
- A opção "contas vencem no mês seguinte" agora vem desmarcada por padrão (conta paga no mês em que foi lançada); pode ser ativada no Calendário.
- Os nomes dos meses voltam a ser os do mês em que a conta foi lançada, sem deslocamento.

## 1.4.1 — 03/11/2026

### Correções
- Importar conta: o mês de destino agora é o mês de referência impresso na conta, não o do vencimento. A conta de energia de Outubro/2026, com vencimento em 06/12, é lançada em Novembro junto com as outras contas de outubro, e o vencimento continua guardado. Na 1.4.0 ela ia para Dezembro.

## 1.4.0 — 03/11/2026

### Novidades
- Mês de pagamento: a tela do mês agora tem o nome do mês em que o dinheiro entra e sai. "Novembro" mostra as contas de outubro (que vencem em novembro) e o salário de outubro (adiantamento do dia 20 e saldo do dia 5). Abas, título e comparações usam esse nome.
- Mês de referência separado do vencimento: ao importar uma conta, o app lê o "Outubro/2026" impresso nela. O consumo (kWh, m³) fica em Outubro, mesmo que a conta só vença em dezembro, e a tela Consumo e os gráficos usam o mês de referência.

### Melhorias
- Importar conta: o diálogo mostra em qual mês a conta vai aparecer, conforme o vencimento (ex.: energia com vencimento em 06/12 aparece em Dezembro), e o mês pode ser trocado ali.
- A fatura da Claro continua lida por rótulos, com os totais por categoria (Internet, TV & Streaming, Celular).

### Correções
- A importação de contas com vencimentos em meses diferentes dava a impressão de apagar a anterior; agora o mês de destino fica explícito antes de importar.

## 1.3.6 — 03/11/2026

### Melhorias
- Importar conta: o diálogo agora explica em qual mês a conta será lançada, conforme o vencimento (ex.: "Vencimento 06/12/2026 → entra em Novembro, paga em Dezembro"), e lembra que o mês pode ser trocado para juntar com as outras contas. O aviso final diz em que mês a conta foi lançada.

### Correções
- Ao importar contas com vencimentos em meses diferentes (ex.: energia vencendo em dezembro e água em novembro), cada uma ia para o seu mês e o app pulava para a última, dando a impressão de que a anterior tinha sido apagada. Nada era apagado; agora o mês de destino fica explícito antes de importar.

## 1.3.5 — 03/11/2026

### Melhorias
- Importar fatura da Claro (e outras contas de telecom/serviços): o app agora lê o valor total pelo rótulo "Total a pagar"/"Valor total", o vencimento, os totais por categoria (Internet, TV & Streaming, Celular) e o código do boleto. A conta é reconhecida como telefone/internet, não mais como cartão.
- Leitura por OCR (PDF escaneado ou foto): os totais por categoria também são reconhecidos quando a linha vem com texto extra colado, comum em OCR.

### Correções
- A fatura da Claro era lida como cartão de crédito e trazia itens errados (datas, linhas de valor 0,00, texto de ofertas). Agora linhas zeradas e o período "01/10/26 A 31/10/26" não viram itens.

## 1.3.4 — 03/11/2026

### Novidades
- Painel fixo "Pago × Em aberto" no fim da lista de contas do mês: ao marcar cada conta como paga, mostra na hora o valor já pago, o que falta pagar, quantas contas faltam e uma barra de progresso.
- Senha com no mínimo 4 caracteres, podendo ser só números (antes eram 6). Vale para criar a senha, trocá-la e redefini-la pelo código de recuperação.

### Melhorias
- Mês de férias na projeção do salário: o salário de cada mês usa a projeção própria dele. Em um mês de férias, o adiantamento do dia 20 e o saldo do dia 5 do mês seguinte já saem reduzidos; o dia 5 do mês de férias traz o saldo integral do mês anterior. O Calendário e a tabela de Pagamento CLT respeitam o mês de férias, e o recibo de férias aparece no Calendário na data em que foi pago (até 2 dias antes do início).
- O Calendário mostra também os adiantamentos e saldos já importados em qualquer mês.
- Importar conta: antes de substituir uma fatura já importada de outro valor na mesma conta e mês, o app pergunta, para não sobrescrever nada sem você ver.

### Correções
- Importar uma conta nova em PDF podia apagar os dados de outra (ex.: importar a conta de água sobrescrevia a de energia). Acontecia quando a calibração guardada de uma conta era aplicada a um PDF de outro tipo; agora o modelo de energia não vale para água, gás, telefone ou cartão.

## 1.3.3 — 03/11/2026

### Novidades
- Opções > "Restaurar o aplicativo do zero": volta o app ao estado de recém-instalado (sem contas, entradas, senha e preferências; você cria uma nova senha). Pede para digitar RESTAURAR, salva um backup antes e não apaga nada de vez: o cofre atual fica guardado na pasta "antes-do-zero", dentro da pasta de backups.

### Melhorias
- Lógica "o que é lançado em um mês é pago ou recebido no mês seguinte" aplicada nas telas: no Início, "Contas a pagar em Novembro" lista as contas lançadas em Outubro (que vencem em novembro), igual ao Calendário. Na tela do mês, os títulos mostram "lançadas em Outubro, pagas em Novembro" e "adiantamento em Outubro, saldo do salário em Novembro".
- O mês anterior continua com a previsão do salário até o holerite ser importado: em Outubro aparece o saldo previsto que cai em 05/11 (o adiantamento do dia 20 já importado não é repetido). Antes, Outubro ficava "no vermelho" por falta dessa previsão.

## 1.3.2 — 02/11/2026

### Melhorias
- Leitura de contas e faturas: o valor total agora é lido do rótulo "Valor total" / "Total a pagar" / "Valor a pagar" (ao lado ou logo abaixo), em vez de somar ou escolher entre valores soltos. Faturas de telefone/internet com várias páginas (ex.: Claro) deixam de ser tratadas como fatura de cartão.
- OCR só quando precisa: em PDFs digitais (com texto de verdade), páginas de capa, propaganda ou imagem não passam mais por OCR no modo automático. Isso deixa a leitura mais rápida e sem lixo. PDFs escaneados continuam usando OCR.
- Calendário: o saldo do salário já recebido aparece no dia certo (ex.: saldo de outubro em 05/11), junto com o adiantamento do dia 20.
- Férias: o recibo de férias conta no mês em que as férias começam, mesmo pago antes (recibo do fim de outubro entra em novembro). Na importação o mês já vem sugerido assim.
- Todas as contas do mês ganharam o botão "+ Boleto/Pix" para guardar a linha digitável ou o Pix copia e cola e exibir o código de barras / QR Code, sem precisar de PDF.

## 1.3.1 — 02/11/2026

### Melhorias
- Férias recebidas antes do mês de gozo: o recibo de férias importado em um mês (ex.: pago no fim de outubro) passa a valer para o mês em que as férias começam (novembro). Esse mês já vem marcado como "Mês de férias" (10 dias trabalhados por padrão, dá para mudar ou desmarcar), com o salário proporcional e sem projetar as férias de novo.
- PDF protegido por senha: o pop-up com "Salvar esta senha" reaproveita a senha na fatura do mês seguinte do mesmo emissor (ex.: Itaú), e as senhas salvas podem ser esquecidas em Segurança.

### Correções
- Contas com vencimento antigo no próprio mês (ex.: conta de outubro com vencimento em outubro) agora aparecem no Calendário no mês seguinte, de acordo com a regra de vencimento no mês seguinte.

## 1.3.0 — 02/11/2026

### Novidades
- Vencimento no mês seguinte: as contas de um mês vencem e são pagas no mês seguinte (as de fevereiro vencem em março). Vale para o Calendário, os avisos de vencimento e a importação de contas (uma conta que vence em março entra em fevereiro). Dá para voltar ao vencimento no próprio mês no Calendário.

### Melhorias
- App mais simples: removidos o acesso pelo celular, a bandeja do sistema (o app não fica mais rodando em segundo plano nem inicia com o Windows), o Windows Hello e o modo discreto. O início automático das versões anteriores é desfeito sozinho.
- "Windows Hello e bloqueio" virou "Bloqueio por inatividade".

## 1.2.1 — 02/11/2026

### Melhorias
- Código de barras e Pix: a tela também abre pelo botão "Código de barras / Pix" na configuração da conta (o chip do tipo da conta), para colar a linha digitável ou o Pix copia e cola à mão.

### Correções
- "Sair e salvar backup" deixava a janela parada em "Salvando o backup…" depois de uma atualização pelo app. O backup já era salvo na hora; agora a janela também fecha sozinha.

## 1.2.0 — 01/11/2026

### Novidades
- Contas parceladas: ao informar as parcelas (ex.: 48), o valor é lançado sozinho em todos os meses até a última parcela, inclusive nos anos seguintes.
- Contas recorrentes: o valor é lançado sozinho nos meses seguintes, sem prazo. Se mudar, é só digitar o novo valor no mês: ele passa a valer dali em diante.
- Código de barras e Pix: ao importar a conta (PDF ou foto), o app guarda a linha digitável do boleto e o Pix copia e cola. O botão "Código de barras" (ou "Pix") na conta mostra o código para escanear pelo app do banco, com opção de copiar. Também dá para colar o código à mão.
- Entradas previstas: do mês atual em diante, cada mês já mostra o adiantamento e o salário previstos pelo último holerite; ao importar o holerite ou o adiantamento, a previsão daquela parte some.
- Projeção do mês: caixinhas para mês de férias (dias trabalhados, com férias + 1/3 e venda de 10 dias) e 13º salário (1ª parcela, 2ª parcela ou parcela única), com o salário bruto do holerite ou informado por você.

### Melhorias
- IA local e Telegram removidos (as configurações que existirem são apagadas do banco).

### Correções
- As configurações do Simulador CLT e o registro do fechamento do mês não ficavam gravados ao reabrir o app.

## 1.1.0 — 30/10/2026

### Novidades
- Windows Hello: desbloqueie com a digital, o rosto ou o PIN do Windows (Opções › Windows Hello e bloqueio). A senha continua valendo e a chave fica no chip de segurança (TPM) do computador.
- Bloqueio por inatividade: o app volta para a tela de senha depois de 1 a 60 minutos sem uso (padrão: 15 minutos).
- Modo discreto: o botão do olho, ao lado de Buscar, esconde os valores da tela (atalho Ctrl+Shift+H). Os relatórios em PDF continuam com os valores.
- Conferência dos backups: cada backup é aberto e conferido logo depois de salvo, ao desbloquear e a cada 6 horas. Se um não abrir, o Início avisa.
- Busca geral (Ctrl+K): encontra contas, itens das faturas e entradas em todos os meses e anos, por nome ou valor.
- Desfazer (Ctrl+Z): volta a última alteração do ano aberto (até 30 alterações).
- Fechamento do mês: roteiro de conferência (faturas, contas pagas, entradas, orçamento) que termina com o PDF de resumo do mês.
- Simulador CLT: mês com 0 a 30 dias trabalhados e o restante de férias (com 1/3 e venda de 10 dias), e o 13º salário na 1ª e na 2ª parcela, com as tabelas de INSS e IRRF de 2026 e os descontos do seu holerite.
- IA local no Meu Consultor Pessoal (opcional): perguntas em linguagem natural respondidas por uma IA que roda no computador (Ollama, gratuito). A IA consulta o app para obter os números; nada sai do computador.
- Telegram (opcional): consultas e relatórios pelo celular de qualquer lugar (/resumo, /contas, /saude, /orcamento, /parcelas, /relatorio ou pergunta livre), com pareamento por código, PIN e mensagens apagadas automaticamente.
- Tema preto (OLED).

### Melhorias
- Celular e bandeja: "Testar a conexão" mostra o tipo da rede, a situação do firewall do Windows e as tentativas de conexão do celular. "Liberar no firewall" cria, com permissão de administrador, uma regra só para a porta do celular e só para a rede local, e pode marcar a rede de casa como privada.
- Instalador confere os requisitos (Windows 10 1809 ou mais novo, 64 bits, Microsoft Edge ou Google Chrome).
- Backups: a lista mostra se cada backup abre normalmente.

### Correções
- Celular: o acesso não funcionava quando a rede do Windows estava como pública ou o firewall não tinha liberação para o app; agora o app mostra o problema e corrige.

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
