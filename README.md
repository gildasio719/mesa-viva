# Mesa Viva

App para a equipe de som da igreja: checklist e diário do culto, chamados do palco, mapa da mesa, fichas da equipe, trilhas de aprendizado, guias de mesas de som e ferramentas do técnico (SOS Microfonia, análise de equilíbrio, medidor de volume, gerador de sinais, treino de ouvido, calculadoras e mapa de frequências).

Protótipo publicado em: https://gildasio719.github.io/mesa-viva/

## Privacidade

- Tudo o que é anotado fica só no aparelho de quem usa, guardado no navegador. Não há servidor nem conta.
- O microfone só liga quando a pessoa toca em "Ouvir ao vivo" ou "Começar a medir", e desliga sozinho ao sair da tela, trocar de ferramenta ou bloquear o celular. O som é analisado no próprio aparelho e não é gravado nem enviado.
- A página proíbe qualquer conexão de rede depois de carregada (`connect-src 'none'` na política de segurança). Mesmo que algum código tentasse enviar dados, o navegador bloquearia.
- As fontes são servidas pelo próprio site, sem chamadas ao Google.

Veja também [SECURITY.md](SECURITY.md).
