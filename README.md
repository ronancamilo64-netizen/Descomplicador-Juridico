# Descomplicador-Juridico
Assistente jurídico com IA para pessoas físicas.Assistente jurídico com IA para pessoas físicas. Analisa contratos (PDF), audita notas fiscais e gera notificações extrajudiciais baseadas no CDC. Desenvolvido com Python, FastAPI e API do Claude (Anthropic). Interface web responsiva sem frameworks frontend
# ⚖️ Descomplicador Jurídico

Assistente jurídico com IA para pessoas físicas. Analisa contratos, audita notas fiscais e gera notificações extrajudiciais baseadas no CDC — tudo em linguagem simples, sem juridiquês.

---

## 💡 O Problema

Quase todo brasileiro já assinou um contrato com medo de uma "cláusula pegadinha" ou não soube como reclamar quando foi lesado por uma empresa. Contratar um advogado para situações do dia a dia é caro e inacessível para a maioria das pessoas.

---

## ✅ Funcionalidades

### 📄 Análise de Contratos
- Envie um PDF de contrato de aluguel ou prestação de serviço
- Recebe um **score de 0 a 100** com pontos de atenção em linguagem simples
- Baseado na Lei do Inquilinato (Lei 8.245/91) e CDC (Lei 8.078/90)

### 🧾 Auditoria de Nota Fiscal
- Confere se os valores da nota batem com os itens cobrados
- Identifica cobranças duplicadas ou taxas suspeitas
- Explica impostos retidos (ISSQN, PIS/COFINS, IRRF) de forma acessível

### ✉️ Gerador de Notificação Extrajudicial
- Transforma um relato informal em uma carta formal com artigos do CDC
- Gera mensagem rápida para o SAC e notificação completa para ouvidoria
- Pronta para enviar ao ReclameAqui ou Juizado Especial Cível

---

## 🛠️ Stack

| Tecnologia | Uso |
|---|---|
| Python 3.x | Backend |
| FastAPI | Servidor HTTP |
| Anthropic Claude API | Processamento com IA |
| HTML / CSS / JS | Interface web (sem frameworks) |
| ngrok | Túnel para acesso mobile |

---

## 🚀 Como Rodar Localmente

### Pré-requisitos
- Python 3.10+
- Conta na [Anthropic](https://console.anthropic.com) com chave de API

### Instalação

```bash
# Clone o repositório
git clone https://github.com/ronancamilo64-netizen/descomplicador-juridico.git
cd descomplicador-juridico

# Instale as dependências
pip install fastapi uvicorn python-multipart PyPDF2 requests
```

### Configuração

Abra o `servidor.py` e substitua a chave de API:

```python
ANTHROPIC_API_KEY = "sk-ant-..."
```

### Execução

```bash
python servidor.py
```

Acesse em: `http://localhost:8000/app`

### Acesso pelo celular (opcional)

```bash
ngrok http 8000
```

Use a URL gerada pelo ngrok no celular — funciona de qualquer rede.

---

## 📁 Estrutura do Projeto

```
descomplicador-juridico/
├── servidor.py       # Backend completo + interface HTML embutida
└── README.md
```

---

## ⚠️ Aviso Legal

Este projeto é um protótipo educacional. As análises geradas pela IA são **informativas** e não substituem a consulta com um advogado habilitado. Não nos responsabilizamos por decisões tomadas com base nas respostas geradas.

---

## 👨‍💻 Autor

Desenvolvido por **Ronan Camilo**  
Especialista em Processos Industriais | Automação | Industry 4.0  
[LinkedIn](https://www.linkedin.com/in/ronancamilo/) · [GitHub](https://github.com/ronancamilo64-netizen)
