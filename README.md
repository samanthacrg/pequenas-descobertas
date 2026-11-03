# Pequenas Descobertas — atividades interativas

Site experimental de atividades de linguagem, brincadeira, compartilhamento e comunicação multimodal, construído para **uso mediado por fonoaudióloga**. A proposta foi inspirada por objetivos clínicos, mas **não inclui PTS, nome, diagnóstico, datas ou informações de pacientes**.

## O que há nesta versão

- 4 atividades: **Olha o que aconteceu**, **Vamos fazer?**, **Faz de conta**, **Minha vez, sua vez!**.
- Sugestões de **palavras essenciais (core words)** específicas para cada atividade, a serem modeladas **no sistema robusto de CAA que a pessoa já utiliza**. Os botões exemplificativos da página não constituem uma prancha de CAA e não substituem o sistema individualizado.
- Voz sintetizada opcional do navegador.
- Registro clínico **somente na memória da aba**, sem login, sem conta e sem banco de dados. Ao fechar/recarregar a página, as observações desaparecem. Você pode exportá-las em arquivo TXT, evitando dados identificáveis.
- Funciona em computador, tablet e celular. Com HTTPS e após o primeiro acesso, os arquivos do site podem ser disponibilizados offline pelo navegador (PWA).

## Como publicar gratuitamente no GitHub Pages

1. Entre em https://github.com e clique em **New repository** (ou **+ → New repository**).
2. Crie um repositório **público** com o nome `pequenas-descobertas`. Não adicione dados de pacientes.
3. No repositório, use **Add file → Upload files** e envie **o conteúdo desta pasta** (não o ZIP): `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, `.gitignore`, `README.md` e a pasta `icons/` com as duas imagens. Ao usar upload web, arquivos ocultos como `.nojekyll` podem exigir criação manual; não é indispensável para esta versão.
4. Clique em **Commit changes**.
5. Vá a **Settings → Pages → Build and deployment → Source → Deploy from a branch**.
6. Selecione **main** e **/(root)** e clique em **Save**.
7. O endereço será `https://SEU_USUARIO.github.io/pequenas-descobertas/` (substitua `SEU_USUARIO`). A disponibilização pode levar alguns minutos.

Para publicar alterações, substitua o `index.html` e os demais arquivos modificados e faça outro commit. Se o navegador não refletir as mudanças imediatamente, recarregue a página.

## Privacidade e limites clínicos

**Importante: GitHub Pages é público.** Mesmo se um repositório privado for permitido no plano, não use o GitHub Pages convencional para hospedar prontuários ou documentos identificáveis. Não publique o PTS original, nomes, fotos, gravações ou registros clínicos pessoais. O site hospeda apenas atividades genéricas. Considere os requisitos de consentimento, sigilo profissional e LGPD antes de levar qualquer informação clínica a um serviço externo.

Os resultados obtidos por toque na tela **não são avaliação padronizada**, e não demonstram por si só aquisição nem generalização de habilidades. A interpretação depende da observação da terapeuta. As intervenções motoras de fala e estratégias PROMPT não foram automatizadas no aplicativo.

**Sem dados enviados por este código**: não há Analytics, login, envio de observações ou servidor de prontuários. Como provedor de hospedagem, o GitHub pode processar dados técnicos de acesso, como endereços IP.

## Desenvolvimento

HTML, CSS e JavaScript em um único `index.html` sem dependências. `manifest.webmanifest` + `sw.js` dão suporte à instalação/uso offline quando o navegador permitir. Você pode editar o código diretamente no GitHub.

## Próximos passos clínicos

- Ajustar cenas e conteúdos às preferências e ao nível atual de compreensão do paciente.
- Escolher palavras essenciais para **modelagem em seu sistema existente**, sem reproduzir a organização da grade ou trocar símbolos arbitrariamente.
- Adicionar modo terapeuta e ferramentas de configuração de atividades, depois de validar o uso clínico.
