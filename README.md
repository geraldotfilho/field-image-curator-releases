# 🏛️ Ateliê Pericial — Central de Releases

Bem-vindo(a) ao repositório oficial de distribuição e download dos executáveis/instaladores prontos para uso do **Ateliê Pericial** (antigamente conhecido como *Field Image Curator*).

O **Ateliê Pericial** é uma suíte desktop integrada de assistência ao perito criminal, desenhada para otimizar e garantir a robustez de todo o fluxo documental da perícia criminal — desde a coleta preliminar de dados do caso e curadoria de vestígios até a renderização do laudo final em formato Word (`.docx`).

---

## 🛠️ O Ecossistema do Ateliê

O aplicativo une três subsistemas funcionais integrados em um único fluxo de trabalho:

1. 📂 **Caso**: Gestão de informações de contexto (REPs, SEIs, partes, datas, locais e georreferenciamento), com preenchimento assistido por dados locais ou planilhas externas.
2. 📸 **Imagens**: Curadoria fotográfica forense ágil e semântica com agrupamento inteligente de fotos (algoritmos locais wHash e embeddings SigLIP), legendagem rápida, transcrição local de áudio (Whisper) e preservação do material original.
3. 📄 **Laudo**: Geração automatizada de laudos periciais formatados e com lógica condicional (Jinja2/docxtpl) com base em modelos customizáveis (`.docx`).

---

## 🚀 Diretrizes do Projeto

* ⚖️ **Autoria Humana Inviolável (P1)**: Toda e qualquer automação, sugestão textual ou indexação local opera apenas como ampliação cognitiva do perito. O julgamento técnico, a análise da dinâmica do fato e as conclusões periciais finais permanecem sob responsabilidade exclusiva e indelegável do perito humano.
* 🔒 **Processamento 100% Local (P3)**: Privacidade absoluta dos dados do caso. Nenhum arquivo, imagem, áudio, descrição ou dado é enviado a servidores na nuvem ou serviços de rede. Toda a inteligência e os modelos rodam off-grid na sua própria máquina.

---

## ⚠️ AVISO IMPORTANTE E DECLARAÇÃO DE RESPONSABILIDADE

> [!WARNING]
> **Software sem Fins Lucrativos e em Desenvolvimento**
>
> 1. **Fase de Testes (Beta)**: Este é um software acadêmico e de testes, de distribuição gratuita e sem fins lucrativos. Ele está em **fase de desenvolvimento ativo**.
> 2. **Use com Cautela**: Por se tratar de uma versão de desenvolvimento, podem ocorrer instabilidades, bugs inesperados ou comportamentos incorretos. **É obrigatório que o usuário revise e valide rigorosamente todo o resultado final** (laudos renderizados, dados salvos, ordenação de imagens e relatórios) antes de qualquer assinatura formal ou uso oficial.
> 3. **Reporte de Bugs**: Contribua para o aprimoramento da ferramenta reportando quaisquer erros ou comportamentos anômalos por meio do menu **Ajuda -> Reportar Bug** no aplicativo ou abrindo uma Issue neste repositório.
> 4. **Isenção de Responsabilidade (Disclaimer)**: O desenvolvedor e os colaboradores deste projeto **não assumem qualquer responsabilidade** por danos diretos, indiretos, perdas de dados de casos criminais, corrupção de mídias, atrasos em relatórios ou conclusões sugeridas. O uso é de responsabilidade técnica exclusiva de quem o opera. Certifique-se de manter cópias de segurança (backups) das suas mídias originais.

---

## 📥 Instruções de Instalação por Plataforma

Os instaladores oficiais e pacotes de release estão disponíveis na aba lateral **[Releases](https://github.com/geraldotfilho/field-image-curator-releases/releases)**. Escolha o instalador da sua plataforma correspondente:

### 🪟 Windows (Recomendado/Suportado Oficialmente)

1. Acesse a página de [Releases](https://github.com/geraldotfilho/field-image-curator-releases/releases) e baixe o arquivo `AteliePericial_Setup.exe` da versão mais recente.
2. Execute o instalador `AteliePericial_Setup.exe` e siga as instruções na tela (será exibida a tela de Termos de Uso).
3. **Integração com o Explorer**: O instalador oferece a opção de se integrar ao menu do botão direito do mouse no Windows Explorer. Assim, você poderá clicar com o botão direito em uma pasta de fotos e selecionar **"Abrir caso do Ateliê nesta pasta"** para iniciar instantaneamente.

> [!IMPORTANT]
> **Ignorando Avisos de Segurança no Windows / Browsers:**
> Como o software é construído de forma independente e sem assinatura digital paga (certificado de desenvolvedor comercial):
> * **No Navegador (Chrome/Edge)**: Ao baixar, o navegador pode alertar que o arquivo "não é baixado com frequência" ou é de "desenvolvedor desconhecido". Clique nas opções de download (reticências ou seta) e selecione **"Manter"** ou **"Manter mesmo assim"**.
> * **No SmartScreen do Windows**: Ao executar o instalador, uma janela azul de alerta de segurança pode aparecer bloqueando o início. Clique no link **"Mais informações"** no corpo do texto da janela e depois no botão **"Executar assim mesmo"** que se tornará visível.

---

### 🐧 Linux

1. Acesse as [Releases](https://github.com/geraldotfilho/field-image-curator-releases/releases) e baixe o pacote compactado para Linux (ex: `AteliePericial_Linux.tar.gz` ou similar).
2. Extraia o conteúdo do pacote em uma pasta de sua escolha.
3. Certifique-se de que possui as dependências do sistema necessárias para a interface gráfica (como bibliotecas gráficas do X11/Wayland e Qt).
4. Torne o executável principal rodável e inicie-o:
   ```bash
   chmod +x AteliePericial
   ./AteliePericial
   ```

---

### 🍏 macOS

1. Acesse as [Releases](https://github.com/geraldotfilho/field-image-curator-releases/releases) e baixe o arquivo de imagem de disco `.dmg` (ou o arquivo `.app` compactado correspondente).
2. Abra o `.dmg` e arraste o ícone do **Ateliê Pericial** para a sua pasta `/Applications` (Aplicativos).

> [!IMPORTANT]
> **Bypass do Gatekeeper no macOS:**
> Devido ao aplicativo não ser assinado na Apple Developer Program:
> 1. Ao tentar abrir o aplicativo pela primeira vez, o macOS exibirá uma mensagem dizendo que o aplicativo "não pode ser aberto porque provém de um desenvolvedor não identificado".
> 2. **Para contornar isso**:
>    * Clique com o **botão direito (ou segure Control)** no ícone do aplicativo na pasta Aplicativos e escolha **Abrir**. Na janela de diálogo que se abre, clique em **Abrir**.
>    * Alternativamente, vá em **Ajustes do Sistema -> Privacidade e Segurança**, role a página até a seção de segurança e clique no botão **"Abrir mesmo assim"** ao lado do aviso sobre o Ateliê Pericial.

---

## 🛠️ Desenvolvimento e Contribuição

* **Distribuição Exclusiva**: Este repositório é utilizado **exclusivamente** para disponibilizar os pacotes compilados (assets de release). Por razões de segurança, integridade das cadeias de custódia e privacidade dos templates forenses de fenda institucional, o código-fonte principal é mantido de forma interna e privada.
* **Sugestões**: Dúvidas, sugestões de novos templates de laudo ou melhorias de UX no agrupamento de imagens podem ser direcionadas abrindo uma Issue.
