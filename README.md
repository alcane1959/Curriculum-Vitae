# CV Atual

Aplicação web local para criação, edição, aprimoramento e exportação de currículos profissionais. O projeto funciona em um único arquivo HTML e não exige instalação, servidor ou conexão com a internet.

## Arquivo principal

`curriculo_backup_importacao_botao_topo.html`

## Principais recursos

- Edição do currículo com pré-visualização em tempo real.
- Geração de resumo profissional conforme a função informada.
- Combinação de uma função principal com uma segunda função ou especialização.
- Formas de combinação:
  - automática;
  - com especialização em;
  - duas funções;
  - atuação integrada.
- Cadastro de experiências profissionais.
- Geração de descrições mais detalhadas para as experiências.
- Cadastro de formação acadêmica e certificações.
- Geração de descrição para a formação.
- Geração de competências técnicas.
- Geração de competências comportamentais.
- Inclusão de idiomas.
- Salvamento automático do último currículo no navegador.
- Exportação do currículo em PDF pela função de impressão do navegador.
- Criação de backup completo em JSON.
- Importação de backup para revisão, correção ou continuação futura.
- Botão para limpar os dados e iniciar um novo currículo.
- Interface responsiva para computador, tablet e celular.

## Como executar

1. Baixe o arquivo `curriculo_backup_importacao_botao_topo.html`.
2. Abra o arquivo em um navegador atualizado, como Microsoft Edge, Google Chrome ou Firefox.
3. Preencha os dados na área de edição.
4. Acompanhe o resultado na prévia do currículo.
5. Use **Exportar PDF** para gerar uma versão pronta para envio.

Não é necessário instalar dependências ou executar comandos.

## Estrutura da aplicação

### Perfil

Permite informar:

- nome completo;
- função principal;
- segunda função ou especialização;
- forma de combinação das funções;
- título profissional combinado;
- cidade;
- telefone;
- e-mail;
- LinkedIn;
- resumo profissional.

O botão **Gerar resumo combinado** cria um texto inicial com base nas funções selecionadas. O conteúdo permanece editável e deve ser revisado antes do uso.

### Experiência

Permite cadastrar múltiplas experiências com:

- cargo;
- empresa;
- período inicial e final;
- ferramentas, indicadores ou resultados;
- descrição das responsabilidades e realizações.

O botão **Gerar texto** cria uma descrição profissional relacionada ao cargo. Mantenha somente atividades e resultados que correspondam à experiência real.

### Formação

Permite cadastrar:

- curso ou certificação;
- instituição;
- ano ou situação de conclusão;
- conhecimentos desenvolvidos;
- descrição da formação.

O botão **Gerar descrição** cria um texto inicial sobre os conhecimentos e aplicações profissionais da formação.

### Competências

A aplicação gera sugestões para:

- competências técnicas;
- competências comportamentais;
- integração entre a função principal e a especialização.

Todos os textos podem ser alterados manualmente.

## Combinação de funções

A aplicação aceita perfis híbridos ou especializados.

Exemplos:

- `Cozinheiro com especialização em Confeitaria`
- `Engenheiro de Aplicação e Vendas Técnicas`
- `Corretor de Imóveis com atuação integrada em Marketing Imobiliário`
- `Técnico Eletrônico e Técnico em Automação Industrial`

Na opção **Automática**, o sistema escolhe uma construção com base na segunda função. Se necessário, selecione manualmente outra forma de combinação ou edite o título final.

## Salvamento automático

O último currículo é salvo automaticamente no armazenamento local do navegador.

Isso permite fechar e abrir novamente o arquivo no mesmo navegador e dispositivo sem perder o preenchimento. O armazenamento local não substitui o backup em arquivo.

O currículo salvo pode não estar disponível quando:

- o histórico ou os dados do navegador forem apagados;
- o arquivo for aberto em outro navegador;
- o arquivo for aberto em outro computador;
- o navegador estiver configurado para eliminar dados locais.

Por segurança, faça backups periódicos.

## Backup do currículo

O botão **Fazer backup** gera um arquivo JSON com os dados do currículo.

O nome segue o padrão:

```text
Nome_Ano_Dia-Mês-Ano_HorahMinuto.json
```

Exemplo:

```text
Maria_Silva_2026_01-11-2026_10h20.json
```

O backup inclui:

- dados do perfil;
- funções e título combinado;
- resumo profissional;
- experiências;
- formações;
- competências;
- idiomas;
- data e hora da geração;
- versão da estrutura do arquivo.

Guarde o JSON em uma pasta segura. O arquivo pode conter informações pessoais.

## Importação de backup

A importação pode ser iniciada de duas maneiras:

- pelo botão **Importar backup** na barra superior;
- pela seção **Backup** da aplicação.

Procedimento:

1. Clique em **Importar backup**.
2. Selecione um arquivo JSON criado pela aplicação.
3. Confira o nome apresentado na confirmação.
4. Confirme a substituição do currículo atual.
5. Revise e edite os dados restaurados.

A importação substitui o conteúdo que estiver aberto. Antes de importar outro currículo, faça backup do conteúdo atual se desejar preservá-lo.

## Exportação para PDF

1. Clique em **Exportar PDF**.
2. Na janela de impressão, escolha **Salvar como PDF**.
3. Selecione o formato A4.
4. Revise margens, escala e quantidade de páginas.
5. Salve o arquivo.

Caso o conteúdo ultrapasse o espaço desejado, reduza textos repetitivos ou ajuste a escala na janela de impressão.

## Novo currículo

O botão **Novo currículo** limpa o currículo atual após uma confirmação.

Antes de usar essa opção, faça um backup se desejar manter os dados existentes. A limpeza não deve ser considerada reversível.

## Privacidade

A aplicação funciona localmente no navegador. Ela não envia automaticamente o currículo para servidores externos.

Mesmo assim, o usuário deve proteger:

- arquivos de backup;
- PDFs exportados;
- dados pessoais armazenados no computador;
- informações sensíveis incluídas nas experiências.

Evite inserir documentos pessoais, dados bancários, senhas ou informações confidenciais desnecessárias.

## Compatibilidade

Recomendado:

- Microsoft Edge atualizado;
- Google Chrome atualizado;
- Mozilla Firefox atualizado.

O navegador precisa permitir:

- JavaScript;
- armazenamento local;
- download de arquivos;
- leitura de arquivo JSON selecionado pelo usuário;
- impressão ou salvamento em PDF.

## Solução de problemas

### Os botões não funcionam

- Confirme que o JavaScript está habilitado.
- Abra o arquivo em um navegador atualizado.
- Baixe novamente o HTML se o arquivo estiver incompleto.
- Evite abrir a página em visualizadores que não executam JavaScript.

### O currículo anterior não apareceu

- Confirme que está usando o mesmo navegador e dispositivo.
- Verifique se os dados de navegação foram apagados.
- Use **Importar backup** para restaurar o JSON salvo.

### O backup não é aceito

- Utilize um arquivo JSON criado pela própria aplicação.
- Não altere manualmente a estrutura do JSON.
- Verifique se o arquivo não está vazio ou corrompido.

### O PDF ficou com muitas páginas

- Revise textos extensos ou repetitivos.
- Remova informações pouco relevantes para a vaga.
- Ajuste a escala e as margens na janela de impressão.

## Boas práticas de uso

- Adapte o currículo para cada oportunidade.
- Use resultados verdadeiros e verificáveis.
- Não inclua ferramentas que você não domina.
- Revise ortografia, datas e contatos.
- Mantenha o título profissional coerente com a experiência.
- Prefira realizações e impactos a listas genéricas de tarefas.
- Faça backup antes de limpar ou importar outro currículo.

## Limitações

- Os textos gerados são sugestões editoriais e não validam experiência profissional.
- O sistema não confirma habilitações, registros profissionais ou requisitos legais.
- O armazenamento automático depende do navegador e do dispositivo.
- A importação aceita a estrutura JSON esperada pela aplicação.
- A exportação em PDF depende das configurações de impressão do navegador.

## Estrutura técnica

- HTML5
- CSS responsivo
- JavaScript puro
- `localStorage` para salvamento automático
- API `Blob` para exportação de backup
- API `FileReader` para importação de backup
- `window.print()` para exportação em PDF

## Versão

Versão inicial documentada: `1.0`

### Instalação no computador

### No Google Chrome ou Microsoft Edge:

  1. Abra o endereço publicado do projeto.
  2. Aguarde o carregamento completo da página.
  3. Clique no ícone de instalação exibido na barra de endereço ou abra o menu do navegador.
  4. Selecione Instalar aplicativo ou Instalar este site como aplicativo.
  5. Confirme a instalação.

Depois disso, o aplicativo poderá ser aberto pelo menu Iniciar, pela área de trabalho ou pelo gerenciador de aplicativos do sistema.

### Instalação no celular ou tablet

### Em navegadores compatíveis:

1. Abra o endereço do projeto.
2. Acesse o menu do navegador.
3. Selecione Instalar aplicativo ou Adicionar à tela inicial.
4. Confirme o nome e a instalação.

O ícone será adicionado à tela inicial do dispositivo.

**Observações**

A disponibilidade e o nome da opção de instalação podem variar conforme o navegador e o sistema operacional.
Abrir somente o arquivo index.html pelo computador não garante a instalação como PWA.
O projeto deve ser publicado em HTTPS para utilizar os recursos completos de instalação e service worker.
O funcionamento offline depende da configuração do service-worker.js e dos arquivos adicionados ao cache.
Atualizações no projeto podem exigir a atualização da versão do cache do service worker.

## Licença e uso

Este projeto pode ser adaptado para uso pessoal. Antes de distribuição pública ou uso comercial, defina uma licença própria e revise os textos, regras de privacidade e responsabilidades aplicáveis.

## Aviso

> Este projeto é uma demonstração educacional desenvolvida para estudos de HTML, CSS e JavaScript. A empresa mencionada é fictícia e qualquer semelhança com empresas reais é mera coincidência.
