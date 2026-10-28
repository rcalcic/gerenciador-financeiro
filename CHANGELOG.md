# Notas de versão

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
