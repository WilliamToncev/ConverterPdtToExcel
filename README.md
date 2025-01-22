Conversor de PDF para Excel

Um script em Python para converter tabelas de um arquivo PDF em uma planilha Excel. Este script utiliza pdfplumber para extrair dados de tabelas e pandas para criar o arquivo Excel.

Funcionalidades
  * Extrai tabelas de arquivos PDF.
  * Suporta PDFs com múltiplas páginas.
  * Salva os dados extraídos em um arquivo Excel.

Requisitos
  * Python 3.6 ou superior
  * Bibliotecas necessárias:
    * pdfplumber
    * pandas
    * openpyxl

Instale as dependências com:
  pip install pdfplumber pandas openpyxl

Como Usar
  1. Clone este repositório ou baixe o script.
  2. Defina os caminhos para o arquivo PDF de entrada e o arquivo Excel de saída desejado no script:
      pdf_path = "caminho_para_seu_arquivo.pdf"
      excel_path = "caminho_para_salvar_arquivo.xlsx"

  3. Execute o script:
      python pdf_to_excel.py

  4. O arquivo Excel será salvo no caminho especificado.

Limitações
  * Funciona melhor com tabelas estruturadas em PDFs.
  * Pode exigir ajustes para PDFs com layouts complexos ou dados não estruturados.

Contribuindo
  * Sinta-se à vontade para enviar issues ou pull requests para melhorar o script.
