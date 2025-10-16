# Guia de Contribuição

Obrigado por considerar contribuir para o Stats-In-Codespace! 🎉

## 🤝 Como Contribuir

### Reportar Problemas

Se você encontrar um bug ou tiver uma sugestão:

1. Verifique se já não existe uma [issue](https://github.com/FGV-Fundacao-Getulio-Vargas/Stats-In-Codespace/issues) similar
2. Crie uma nova issue com:
   - Título descritivo
   - Descrição detalhada do problema ou sugestão
   - Passos para reproduzir (se for um bug)
   - Screenshots ou logs (se aplicável)

### Submeter Alterações

1. **Fork o repositório**
   - Clique em "Fork" no canto superior direito

2. **Clone seu fork**
   ```bash
   git clone https://github.com/SEU-USUARIO/Stats-In-Codespace.git
   cd Stats-In-Codespace
   ```

3. **Crie uma branch**
   ```bash
   git checkout -b feature/minha-contribuicao
   ```

4. **Faça suas alterações**
   - Mantenha as alterações focadas e específicas
   - Siga as convenções de código existentes
   - Teste suas alterações

5. **Commit suas alterações**
   ```bash
   git add .
   git commit -m "Descrição clara da alteração"
   ```

6. **Push para seu fork**
   ```bash
   git push origin feature/minha-contribuicao
   ```

7. **Abra um Pull Request**
   - Vá para o repositório original
   - Clique em "New Pull Request"
   - Descreva suas alterações detalhadamente

## 📝 Diretrizes

### Código

- Use nomes descritivos para variáveis e funções
- Adicione comentários quando necessário
- Mantenha compatibilidade com versões anteriores quando possível

### Notebooks

- Inclua células Markdown explicativas
- Use dados de exemplo quando possível
- Certifique-se de que todas as células executam sem erros

### Documentação

- Use linguagem clara e simples
- Inclua exemplos quando apropriado
- Mantenha a formatação consistente

### Commits

Formato sugerido:
```
tipo: descrição curta

Descrição mais detalhada se necessário.
```

Tipos:
- `feat`: Nova funcionalidade
- `fix`: Correção de bug
- `docs`: Mudanças em documentação
- `style`: Formatação, sem mudança de código
- `refactor`: Refatoração de código
- `test`: Adição ou correção de testes
- `chore`: Tarefas de manutenção

## 🎯 Áreas de Contribuição

### Alta Prioridade

- [ ] Adicionar mais notebooks de exemplo
- [ ] Melhorar documentação em português
- [ ] Adicionar testes automatizados
- [ ] Otimizar tempo de setup

### Novas Funcionalidades

- [ ] Suporte para Julia
- [ ] Integração com bancos de dados
- [ ] Templates de análises comuns
- [ ] Datasets de exemplo

### Melhorias

- [ ] Adicionar mais pacotes R úteis
- [ ] Adicionar mais pacotes Python
- [ ] Melhorar mensagens de erro no setup
- [ ] Adicionar troubleshooting guide

## 🧪 Testando Alterações

### Testar Localmente

1. Abra o repositório no VS Code
2. Quando solicitado, "Reopen in Container"
3. Aguarde o setup completar
4. Teste suas alterações

### Testar no Codespaces

1. Crie um Codespace do seu fork
2. Aguarde o setup
3. Verifique se tudo funciona

### Validação Automática

O repositório possui GitHub Actions que validam:
- Sintaxe JSON dos arquivos de configuração
- Permissões dos scripts
- Existência de arquivos necessários

## 📚 Recursos para Contribuidores

### Documentação Útil

- [Dev Containers](https://containers.dev/)
- [GitHub Codespaces](https://docs.github.com/en/codespaces)
- [Jupyter Notebooks](https://jupyter-notebook.readthedocs.io/)
- [IRkernel](https://irkernel.github.io/)

### Ferramentas

- [VS Code](https://code.visualstudio.com/)
- [Docker Desktop](https://www.docker.com/products/docker-desktop)
- [GitHub CLI](https://cli.github.com/)

## ✅ Checklist antes de Submeter

- [ ] Código testado localmente
- [ ] Documentação atualizada
- [ ] Exemplos funcionando
- [ ] Commits organizados
- [ ] Pull request com descrição clara
- [ ] Sem conflitos com branch main

## 🎓 Primeiras Contribuições

Se esta é sua primeira contribuição para projetos open source:

1. Comece com algo pequeno
2. Leia toda a documentação
3. Não tenha medo de fazer perguntas
4. Seja paciente com revisões

Algumas sugestões de primeiras contribuições:
- Corrigir typos na documentação
- Melhorar exemplos existentes
- Adicionar comentários ao código
- Traduzir documentação

## 🙏 Agradecimentos

Toda contribuição é valorizada! Obrigado por ajudar a melhorar este projeto.

## 📞 Contato

Se tiver dúvidas sobre contribuições:
- Abra uma [issue](https://github.com/FGV-Fundacao-Getulio-Vargas/Stats-In-Codespace/issues)
- Inicie uma [discussão](https://github.com/FGV-Fundacao-Getulio-Vargas/Stats-In-Codespace/discussions)

---

**Nota**: Este é um projeto educacional. Mantenha o foco em facilitar o aprendizado de estatística e ciência de dados.
