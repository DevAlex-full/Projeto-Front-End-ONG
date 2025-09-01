# PataAmiga 🐾

> **ONG de Proteção Animal** - Dê um lar para quem precisa de amor

Um site responsivo e moderno desenvolvido para uma ONG fictícia de proteção animal, focado na promoção de adoção responsável e conscientização sobre bem-estar animal.

## 📋 Sobre o Projeto

O PataAmiga é um projeto web que simula o site de uma ONG de proteção animal, desenvolvido com foco em:

- **Adoção Responsável**: Showcase de animais disponíveis para adoção
- **Conscientização**: Informações sobre bem-estar animal e guarda responsável
- **Transparência**: Estatísticas e informações sobre o trabalho da organização
- **Engajamento**: Múltiplas formas de contribuição e voluntariado

### 🎯 Funcionalidades

- ✅ Design responsivo para todos os dispositivos
- ✅ Navegação suave entre seções
- ✅ Menu hambúrguer para dispositivos móveis
- ✅ Galeria de animais para adoção
- ✅ Formulário de contato funcional
- ✅ Seções informativas sobre serviços
- ✅ Estatísticas de impacto da organização

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura semântica e acessível
- **CSS3** - Estilização responsiva e moderna
- **JavaScript ES6+** - Interatividade e funcionalidades dinâmicas

### 📁 Estrutura do Projeto

```
pataamiga/
├── index.html              # Página principal
├── src/
│   ├── styles/
│   │   ├── reset.css       # Reset de estilos
│   │   └── main.css        # Estilos principais
│   └── index.js            # Scripts JavaScript
└── README.md               # Documentação
```

## 🚀 Como Executar

### Pré-requisitos

- Navegador web moderno
- Servidor local (opcional, para desenvolvimento)

### Instalação

1. **Clone o repositório**
   ```bash
   git clone https://github.com/seu-usuario/pataamiga.git
   cd pataamiga
   ```

2. **Execute localmente**
   
   **Opção 1: Abrir diretamente**
   - Abra o arquivo `index.html` no seu navegador

   **Opção 2: Servidor local (recomendado)**
   ```bash
   # Com Python 3
   python -m http.server 8000
   
   # Com Node.js (http-server)
   npx http-server
   
   # Com PHP
   php -S localhost:8000
   ```

3. **Acesse no navegador**
   ```
   http://localhost:8000
   ```

## 📱 Responsividade

O projeto foi desenvolvido com abordagem **mobile-first** e inclui:

- **Desktop** (1200px+): Layout em grid completo
- **Tablet** (768px - 1199px): Layout adaptado
- **Mobile** (até 767px): Menu hambúrguer e layout em coluna única

### Breakpoints principais:
- `max-width: 768px` - Transição para layout mobile
- `max-width: 480px` - Otimizações para telas pequenas

## 🎨 Design System

### Paleta de Cores
- **Verde Principal**: `#4CAF50` - CTAs e elementos destacados
- **Verde Escuro**: `#388E3C` - Navegação e hover states
- **Verde Muito Escuro**: `#2E7D32` - Textos e elementos de ênfase
- **Fundo Claro**: `#f9f9f9` - Background geral
- **Verde Suave**: `#E8F5E9` - Seções e cards

### Tipografia
- **Fonte Principal**: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
- **Hierarquia**: H1 (2.5rem) → H2 (2rem) → H3 (padrão)

## 📊 Seções do Site

### 🏠 Home
Banner principal com call-to-action para adoção

### ℹ️ Sobre Nós
- História da organização
- Missão e valores
- Estatísticas de impacto

### 🐕 Adoção
Galeria de animais disponíveis com:
- Fotos dos animais
- Informações básicas (nome, idade, sexo)
- Status de vacinação/castração

### 🛠️ Serviços
- Resgate de animais
- Atendimento veterinário
- Programa de castração
- Educação e conscientização
- Apadrinhamento

### 🤝 Como Ajudar
Múltiplas formas de contribuição:
- Adoção
- Doações financeiras
- Doação de itens
- Voluntariado
- Lar temporário
- Divulgação

### 📞 Contato
Formulário completo com:
- Validação de campos obrigatórios
- Categorização por assunto
- Design acessível

## 🔧 Funcionalidades JavaScript

### Menu Mobile
```javascript
// Toggle do menu hambúrguer
document.querySelector('.menu-toggle').addEventListener('click', function () {
    document.querySelector('nav ul').classList.toggle('active');
});
```

### Navegação Suave
```javascript
// Scroll suave para âncoras internas
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        document.querySelector(this.getAttribute('href')).scrollIntoView({
            behavior: 'smooth'
        });
        // Auto-fecha menu mobile
        document.querySelector('nav ul').classList.remove('active');
    });
});
```

## 🎯 Melhorias Futuras

### Funcionalidades Planejadas
- [ ] Integração com banco de dados para animais
- [ ] Sistema de busca e filtros
- [ ] Área administrativa para gestão
- [ ] Blog/notícias
- [ ] Sistema de agendamento
- [ ] Integração com redes sociais
- [ ] Galeria de fotos mais robusta
- [ ] Sistema de doações online

### Otimizações Técnicas
- [ ] Implementação de PWA
- [ ] Otimização de imagens (WebP)
- [ ] Lazy loading
- [ ] Minificação de assets
- [ ] Implementação de cache
- [ ] Análise de performance

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

### 📝 Padrões de Código
- Use indentação de 4 espaços
- Mantenha comentários em português
- Siga as convenções de nomenclatura existentes
- Teste em diferentes navegadores e dispositivos

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

### 🐾 Sobre a Causa

Este projeto foi criado para demonstrar como a tecnologia pode ser usada para causas sociais importantes. A proteção animal é uma causa que merece nossa atenção e apoio.

**"Até que um tenha amado um animal, uma parte da alma permanece adormecida."** - Anatole France

---

⭐ **Se este projeto foi útil para você, deixe uma estrela!**
