# Segurança

## Como o app se protege

- **Política de segurança de conteúdo (CSP):** só executa os scripts do próprio arquivo, liberados por hash; bloqueia qualquer conexão de rede (`connect-src 'none'`), formulários externos, plugins e mudança de `base`.
- **Sem dependências de terceiros:** nenhuma biblioteca externa é carregada. As fontes ficam na pasta `fonts/`.
- **Proteção contra ser embutido:** se a página for aberta dentro de outro site (iframe), ela se esconde e tenta abrir no endereço próprio.
- **Dados locais validados:** o que vem do armazenamento do navegador é conferido e limitado em tamanho antes de ser usado, e todo texto digitado é escapado antes de aparecer na tela.
- **Microfone sob controle:** liga só por ação da pessoa, mostra um aviso enquanto está ligado e desliga ao sair da tela, ao trocar de ferramenta, ao bloquear o celular ou depois de 30 minutos.
- **Sem indexação:** a página pede aos buscadores para não indexá-la.

## Limites conhecidos

- O GitHub Pages não permite configurar cabeçalhos HTTP, então algumas proteções ficam na própria página (meta CSP e o bloqueio de iframe em JavaScript).
- O repositório é público: nunca coloque senhas, chaves ou dados de pessoas aqui.

## Boas práticas para quem mantém

- Ative a verificação em duas etapas na conta do GitHub.
- Mantenha o app do Claude no GitHub com acesso só a este repositório.
- Em Settings > Pages, deixe "Enforce HTTPS" ligado.

## Reportar um problema

Abra uma issue sem detalhes sensíveis ou fale diretamente com o mantenedor.
