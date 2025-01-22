import pdfplumber
import pandas as pd

def pdf_to_excel(pdf_path, excel_path):
    try:
        # Abre o arquivo PDF
        with pdfplumber.open(pdf_path) as pdf:
            data = []  # Lista para armazenar os dados extraídos
            
            # Itera sobre todas as páginas do PDF
            for page in pdf.pages:
                # Extraindo tabelas da página atual
                tables = page.extract_tables()

                for table in tables:
                    for row in table:
                        data.append(row)

        # Converte os dados extraídos para um DataFrame do pandas
        df = pd.DataFrame(data)

        # Salva o DataFrame em um arquivo Excel
        df.to_excel(excel_path, index=False, header=False)

        print(f"Arquivo Excel salvo com sucesso em: {excel_path}")

    except Exception as e:
        print(f"Erro ao converter PDF para Excel: {e}")

# Caminhos dos arquivos PDF de entrada e Excel de saída
pdf_path = "NOME_ARQUIVO.pdf"
excel_path = "NOME_ARQUIVO).xlsx"

# Chama a função para converter
pdf_to_excel(pdf_path, excel_path)
