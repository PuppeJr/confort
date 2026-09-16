# 🕶️ Compatibilidade & Conforto

Uma ferramenta interativa para analisar a compatibilidade entre sua receita oftalmológica e a armação de óculos que você deseja usar. Saiba se a combinação escolhida será confortável e adequada!

## 📋 Sobre o Projeto

O **Confort** é um analisador de compatibilidade e conforto visual que ajuda você a:

- ✅ Verificar se sua receita é compatível com a armação escolhida
- 📏 Estimar a espessura das lentes e seus efeitos
- 👁️ Calcular como seus olhos aparecerão (magnificação estética)
- 🔍 Identificar problemas potenciais antes de encomendar os óculos
- ⭐ Receber um score de conforto de 0 a 10
- 📷 Estimar proporções do rosto usando a câmera do dispositivo

## 🚀 Como Usar

1. Acesse a aplicação (hospedada em Vercel)
2. Preencha as informações de sua **receita oftalmológica**:
   - Esfera (grau)
   - Cilindro (astigmatismo)
   - Eixo
   - Distância entre pupilas (DNP)
   - Distância olho-lente
   - Tipo de lente (monofocal/multifocal)
   - Material da lente (índice de refração)

3. Preencha os dados da **armação escolhida**:
   - Largura da lente
   - Ponte
   - Altura da lente
   - Tipo de aro (fechado, semiaberto, rimless)
   - Curvatura da armação

4. Clique em **"🔍 Analisar Compatibilidade e Conforto"**

5. Veja o resultado com:
   - Status geral (Compatível ✅ / Requer Atenção ⚠️ / Não Recomendado ❌)
   - Score de conforto visual (0-10)
   - Análise detalhada de cada fator
   - Detalhes técnicos da combinação

6. Opcionalmente, clique em **"📷 Iniciar câmera"** para medir as proporções faciais:
   - Permita o acesso à câmera
   - Posicione o rosto de frente e clique em **"📏 Medir meu rosto"**
   - Confira a largura e a altura estimadas do rosto e a comparação com a armação informada

## 📊 Critérios Analisados

### 1. **Espessura x Tipo de Aro**
   - Valida se a espessura estimada é adequada para o tipo de aro escolhido
   - Para aros fechados: penaliza lentes muito grossas
   - Para rimless: alerta sobre risco de quebra se muito fina
   - Para semiabertos: verifica fixabilidade no fio

### 2. **Centralização (Decentração)**
   - Calcula se a distância entre pupilas combina com a armação
   - Alerta se será necessário bloco especial (mais caro)

### 3. **Magnificação Estética**
   - Estima quanto seus olhos parecerão maiores ou menores
   - Importante para graus altos (±4D ou mais)

### 4. **Multifocais (Progressivas)**
   - Verifica altura mínima da lente (24mm recomendado)
   - Analisa curvatura da armação (máx 8° recomendado)
   - Avisa se o campo de perto será reduzido

### 5. **Otimização de Custo**
   - Recomenda índices mais simples para graus baixos
   - Evita pagar por materiais ultra-finos desnecessários

## 💡 Tecnologia

- **HTML5** com semântica completa
- **CSS3** responsivo e moderno
- **JavaScript puro** (vanilla JS) sem dependências
- **MediaPipe Face Landmarker** carregado no navegador para detectar pontos faciais
- **Hospedagem**: Vercel
- Cálculos ópticos baseados em fórmulas de ótica oftalmológica

## 📁 Estrutura

```
confort/
├── index.html       # Aplicação completa (HTML + CSS + JS)
├── vercel.json      # Configuração de deploy no Vercel
├── .gitignore       # Arquivos ignorados pelo Git
└── README.md        # Este arquivo
```

## 🔧 Instalação Local

```bash
# Clonar o repositório
git clone https://github.com/PuppeJr/confort.git

# Navegar para o diretório
cd confort

# Abrir no navegador (nenhuma dependência necessária)
# Abra o arquivo index.html em seu navegador
```

## 📱 Responsividade

A aplicação é totalmente responsiva e funciona em:
- 💻 Computadores
- 📱 Tablets
- 📞 Smartphones

## ⚠️ Informações Importantes

- **Esta não é uma ferramenta diagnóstica médica**. Use como referência complementar.
- Consulte sempre um oftalmologista para prescrições e recomendações finais.
- Os cálculos são estimativas baseadas em óptica oftalmológica padrão.
- Diferentes fabricantes podem ter variações em suas medidas.
- A análise da câmera usa a DNP informada como referência de escala e não substitui uma medição profissional.
- Nesta primeira versão, a câmera mede proporções faciais; a identificação automática do contorno dos óculos será adicionada posteriormente.

## 🎯 Interpretação dos Resultados

### ✅ Compatível (8-10 pontos)
Excelente combinação! Você pode prosseguir com confiança. Poucas ou nenhuma observação.

### ⚠️ Requer Atenção (5-7 pontos)
A combinação funciona, mas há pontos que podem afetar seu conforto. Leia os detalhes e considere alternativas.

### ❌ Não Recomendado (0-4 pontos)
Essa combinação tem problemas sérios. Recomenda-se trocar a armação ou o tipo de lente.

## 🤝 Contribuições

Sugestões de melhorias são bem-vindas! Abra uma issue ou pull request.

## 📄 Licença

Sem licença especificada no momento.

## 👨‍💻 Autor

Desenvolvido por [PuppeJr](https://github.com/PuppeJr)

---

**Última atualização**: Julho de 2026

Boa sorte na escolha dos seus óculos! 👓
