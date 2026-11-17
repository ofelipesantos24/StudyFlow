# StudyFlow

Crie planos de estudo e acompanhe o seu aprendizado, tudo no navegador, sem instalação e sem cadastro.

## O que ele faz

- **Cria planos de estudo:** você informa a matéria, a data final e a lista de tópicos. O StudyFlow distribui os tópicos em datas sugeridas, de hoje até o prazo.
- **Acompanha o progresso:** marque cada tópico como concluído e veja a barra de progresso do plano.
- **Avisa sobre atrasos:** tópicos não concluídos depois da data sugerida aparecem como "atrasado".
- **Registra o tempo de estudo:** anote os minutos estudados em cada plano.
- **Mostra um resumo geral:** número de planos, percentual de tópicos concluídos e total de minutos.
- **Salva automaticamente:** os dados ficam no `localStorage` do seu navegador.

## Como usar

1. Abra o arquivo `index.html` em qualquer navegador moderno (basta dar dois cliques).
2. No painel **Novo plano**, preencha o nome, a data final e os tópicos (um por linha).
3. Clique em **Criar plano**.
4. Marque os tópicos conforme estuda e use **Registrar estudo** para somar minutos.

## Estrutura do projeto

```
studyflow/
├── index.html   # aplicação completa (HTML, CSS e JavaScript)
└── README.md    # esta documentação
```

## Tecnologias

- HTML, CSS e JavaScript puro, sem dependências nem etapa de build
- `localStorage` para persistência
- Fontes Bricolage Grotesque e Source Serif 4 (Google Fonts, com fallback para fontes do sistema)
- Tema claro e escuro automático, conforme o sistema

## Como as datas são calculadas

Se o plano tem `N` tópicos e `D` dias até o prazo, o tópico de posição `i` recebe a data `hoje + D × i / N`. O último tópico fica sempre na data final.

## Limitações

- Os dados ficam só no navegador e no dispositivo em que foram criados. Limpar os dados do site apaga os planos.
- Não há edição de plano: para mudar algo, exclua e crie de novo.

## Ideias para evoluir

- Editar planos e tópicos
- Exportar e importar dados em JSON
- Meta semanal de horas e gráfico de evolução
- Lembretes e revisão espaçada
- Sincronização entre dispositivos

## Licença

MIT. Use e modifique à vontade.
