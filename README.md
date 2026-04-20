# Field Image Curator (Windows Releases)

Bem-vindo(a) ao repositório oficial de distribuição do **Field Image Curator**.

Este aplicativo foi desenhado para **curadoria forense e processamento de imagens de campo**, entregando um fluxo de trabalho extremamente rápido para agrupar, filtrar e exportar lotes massivos de fotografias.

## ✨ Principais Funcionalidades

- **Layout Dinâmico e Responsivo**: A interface se adapta perfeitamente a qualquer monitor, gerenciando fotos gigantescas sem estourar a memória RAM do computador.
- **Modo Pilha (Stacking)**: Agrupe múltiplas imagens do mesmo vestígio ou local (ex: foto bruta e versão demarcada).
- **Salvamento**: O estado do seu projeto é guardado para que possa continuar depois.
- **Exportação Forense**: Cria um relatório final em formato Markdown (`contexto.md`), organiza todas as fotos aprovadas sequencialmente em uma pasta `curadoria_final` e insere os metadados EXIF.

---

## 📥 Download e Instalação

As versões prontas para uso estão sempre publicadas na aba lateral do GitHub (Releases).

1. Acesse a página de [Releases](https://github.com/geraldotfilho/field-image-curator-releases/releases).
2. Expanda o item **Assets** da versão mais recente.
3. Baixe o arquivo `FieldImageCurator_Setup.exe`.
4. Execute o instalador no seu computador Windows (suporte oficial para Windows 11).

### Teste Rápido no Windows
A instalação possui também integração com o menu de contexto ("Botão Direito") do Windows Explorer, agilizando drasticamente o início de novos projetos ao clicar com o botão direito em uma pasta e escolher "Curadoria destas Imagens".

---

> [!NOTE]
> **Aviso sobre o Código-Fonte:**
> Este repositório é utilizado **exclusivamente** para a distribuição pública dos instaladores Windows binários (.exe) aos colegas, usuários e parceiros de teste. Todo o código-fonte (Python/PySide6) e a pipeline de CI/CD do sistema são mantidos fechados em um repositório interno de desenvolvimento por motivos de segurança e integridade do projeto. Qualquer dúvida pode ser esclarecida diretamente com o desenvolvedor.
> Atenção! Estão sendo disponibilizadas algumas versões ainda em estágio de testes. Use sob seu próprio crivo e risco. Não me responsabilizo por eventuais prejuízos.
