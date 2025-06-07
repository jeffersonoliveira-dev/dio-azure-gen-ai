# **Desafio DIO: Explorando Copilot e OpenAI**

## **Descrição do Projeto**  
Este repositório documenta minha experiência prática com **Microsoft Copilot** e **OpenAI**, explorando suas funcionalidades, filtros de conteúdo e recursos de criação assistida por IA. O objetivo foi aplicar os conceitos aprendidos nas aulas da DIO e registrar os resultados obtidos.

---

## **Objetivos Alcançados**  
✅ Configuração e uso do **Microsoft Copilot** em diferentes cenários  
✅ Exploração do **Azure OpenAI Service** (GPT-4, embeddings, filtros de conteúdo)  
✅ Criação de **prompts eficientes** para geração de texto, código e análise de dados  
✅ Implementação de **filtros de segurança** para moderar saídas da IA  
✅ Documentação dos aprendizados e exemplos práticos  

---

## **Tecnologias Utilizadas**  
- **Microsoft Copilot** (Copilot Studio, GitHub Copilot)  
- **Azure OpenAI Service** (GPT-4, DALL·E, embeddings)  
- **Prompt Engineering** (técnicas para melhorar respostas da IA)  
- **Filtros de Conteúdo** (moderação de saídas sensíveis)  

---

## **Passo a Passo**  

### **1. Configuração do Ambiente**  
- Criei um recurso **Azure OpenAI Service** no portal da Microsoft  
- Acessei o **Copilot Studio** para personalizar assistentes virtuais  
- Configurei **GitHub Copilot** para auxílio em desenvolvimento de código  

### **2. Experimentando o Microsoft Copilot**  
Testei diferentes funcionalidades:  
- **Copilot no VS Code** (geração de código, explicação de trechos)  
- **Copilot no Teams** (resumo de reuniões, geração de atas)  
- **Copilot no Edge** (pesquisa inteligente, síntese de artigos)  

📌 **Exemplo de Prompt:**  
```
"Explique como otimizar uma consulta SQL com JOINs e sugira melhorias no seguinte código: [código]"
```

### **3. Explorando Azure OpenAI**  
- Utilizei o **GPT-4** para:  
  - Gerar textos criativos  
  - Responder perguntas técnicas  
  - Traduzir e resumir documentos  
- Testei o **DALL·E** para geração de imagens a partir de descrições  
- Apliquei **embeddings** para busca semântica em documentos  

📌 **Exemplo de Uso do GPT-4:**  
```python
import openai

response = openai.ChatCompletion.create(
    model="gpt-4",
    messages=[{"role": "user", "content": "Explique o conceito de machine learning em 3 linhas"}]
)
print(response.choices[0].message.content)
```

### **4. Filtros de Conteúdo e Segurança**  
Configurei filtros no Azure OpenAI para:  
- **Moderação de conteúdo ofensivo**  
- **Prevenção de vazamento de dados sensíveis**  
- **Controle de tópicos restritos**  

📌 **Exemplo de Filtro:**  
```json
{
  "filter_categories": ["hate", "violence", "self-harm"],
  "filter_strength": "medium"
}
```

---

## **Resultados e Insights**  
🔹 **Copilot** aumenta produtividade em codificação e documentação  
🔹 **Prompt Engineering** é essencial para respostas precisas  
🔹 **Filtros de conteúdo** evitam saídas inadequadas  
🔹 **GPT-4** é poderoso, mas requer instruções claras  

---

## **Desafios Encontrados**  
⚠️ **Latência** em respostas do GPT-4 em requisições complexas  
⚠️ Necessidade de ajuste fino em **prompts** para melhores resultados  
⚠️ Limitações em **context length** (tamanho do texto de entrada)  

---

## **Próximos Passos**  
- [ ] Integrar **OpenAI em um chatbot** personalizado  
- [ ] Testar **fine-tuning** para domínios específicos  
- [ ] Explorar **automações com Copilot Studio**  

---

## **Referências Úteis**  
- [Documentação do Azure OpenAI](https://learn.microsoft.com/azure/ai-services/openai/)  
- [Copilot Studio](https://learn.microsoft.com/copilot-studio/)  
- [Prompt Engineering Guide](https://learn.microsoft.com/azure/ai-services/openai/concepts/prompt-engineering)  

---

### **Conclusão**  
Este projeto me permitiu explorar na prática o potencial do **Copilot e OpenAI**, desde geração de conteúdo até aplicações em desenvolvimento de software. O repositório serve como base para futuras implementações e consulta.  
