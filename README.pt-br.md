# Live Option Price for OpenCart 3.x / 4.x

![Versão do OpenCart](https://img.shields.io/badge/OpenCart-4.x-blue?style=for-the-badge&logo=opencart)
![Versão do OpenCart](https://img.shields.io/badge/OpenCart-3.x-blue?style=for-the-badge&logo=opencart)
![Licença](https://img.shields.io/badge/License-GPL--3.0-green?style=for-the-badge)
![Idiomas](https://img.shields.io/badge/Languages-5-orange?style=for-the-badge)

[English](README.md) | [Português (BR)](README.pt-br.md) | [Português (PT)](README.pt-pt.md) | [Español](README.es-es.md) | [Français](README.fr-fr.md) | [Italiano](README.it-it.md)

![Live Option Price](./assets/images/social_preview.png)

[![Download](./assets/images/pt-br/download.png)](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## Sobre

### Visão geral

<p align="center">
  <img src="./assets/images/demo-price-animation.gif" width="20%" />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="./assets/images/demo-fade-effect.gif" width="20%" />
</p>

O **Live Option Price** atualiza o preço do produto em tempo real conforme o cliente seleciona suas opções, altera a quantidade ou modifica outras informações relacionadas ao produto.

Sem o módulo, o preço exibido na página do produto pode permanecer inalterado até que o cliente conclua uma ação adicional. Com o **Live Option Price**, os valores são recalculados automaticamente e apresentados diretamente na página do produto.

O módulo utiliza os valores configurados nativamente no OpenCart, incluindo:

- Preço do produto.
- Preço das opções.
- Descontos.
- Preço especial.
- Impostos.
- Pontos do produto e das opções, quando habilitado.
- Quantidade selecionada.

O resultado é apresentado diretamente na página do produto, proporcionando ao cliente uma visualização imediata do valor correspondente à configuração escolhida.

### Compatibilidade

O **Live Option Price** foi desenvolvido para funcionar nas versões:

- **OpenCart 3.x**
- **OpenCart 4.x**

A interface administrativa e o funcionamento podem apresentar pequenas diferenças visuais entre as versões do OpenCart, mas os recursos e as configurações do módulo permanecem os mesmos.

---

## Requisitos

Certifique-se de possuir permissões administrativas para:

- **Instalador de Extensões**
- **Extensões / Módulos**
- **Modificações**
- **Configuração do módulo**

> **Importante:** a instalação deve ser realizada utilizando o arquivo oficial do módulo fornecido para sua versão do OpenCart.

---

## Principais recursos

| Recurso | Descrição |
| :--- | :--- |
| **Preço em tempo real** | Atualiza o preço automaticamente quando o cliente altera as opções do produto. |
| **Preços das opções** | Considera os acréscimos e descontos definidos nas opções do produto. |
| **Descontos por quantidade** | Considera automaticamente os descontos por quantidade configurados no OpenCart. |
| **Preço especial** | Mantém o cálculo compatível com o preço especial do produto. |
| **Multiplicação pela quantidade** | Permite exibir o valor total de acordo com a quantidade selecionada. |
| **Preço unitário** | Exibe o preço correspondente a uma unidade quando o cliente seleciona mais de uma unidade. |
| **Selo de desconto** | Exibe visualmente a porcentagem de desconto aplicada ao produto. |
| **Impostos** | Atualiza a informação de preço relacionada aos impostos conforme a configuração fiscal do OpenCart. |
| **Pontos** | Atualiza os pontos exibidos para o produto conforme as opções selecionadas e a quantidade. |
| **Animação de contagem** | Anima a alteração numérica do preço durante as atualizações. |
| **Efeito de opacidade** | Aplica uma transição visual durante a atualização do preço. |

---

> **Importante:** o módulo não substitui a configuração de preços do OpenCart. Ele utiliza os valores existentes no produto, nas opções, nos descontos e nas configurações fiscais da loja para realizar o cálculo.

---

## Instalação

Siga o fluxo abaixo para aplicar a numeração automática aos seus produtos:

1. **Download**: Obtenha o módulo oficial diretamente no [OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr).
2. **Upload**: No painel administrativo da sua loja, acesse **Extensions > Installer**, clique em **Upload** e selecione o arquivo baixado.
3. **Ativação**: Localize o módulo na lista de extensões e clique no ícone **Install** para ativá-lo.

> **Dica técnica**: Após a ativação, lembre-se de acessar **Extensions > Modifications** e clicar no botão **Refresh** (ícone azul) para limpar o cache do sistema.

---

## Acessando as configurações

Depois de instalar o módulo:

1. Acesse **Extensões > Extensões**.
2. Filtre por **Módulos**.
3. Localize **Live Option Price**.
4. Clique em **Editar**.

---

# Configurações

![Configuração](./assets/images/pt-br/docs-config-pt-br.png)

| Parâmetro | Função |
|---|---|
| **Multiplicar pela quantidade** | Determina se o preço exibido deverá considerar a quantidade selecionada pelo cliente.<br>**Importante:** esta configuração controla especificamente a forma como o preço é apresentado. A quantidade continua sendo considerada pelo OpenCart nas demais operações aplicáveis. |
| **Exibir selo de desconto** | Exibe um selo com a porcentagem de desconto quando o produto possui um preço promocional ou desconto por quantidade aplicável.<br>**Importante:** o percentual apresentado é calculado pelo módulo com base na diferença entre o preço utilizado como referência e o preço com desconto aplicado. |
| **Exibir preço unitário** | Exibe o valor correspondente a uma unidade do produto quando a quantidade selecionada for maior que 1. O preço unitário é exibido quando o cálculo está configurado para considerar a quantidade e a quantidade selecionada é superior a uma unidade.<br>**Observação:** esta função apenas atualiza a informação apresentada dinamicamente na página do produto. As regras de pontos do OpenCart continuam sendo a fonte dos valores utilizados pelo módulo. |
| **Calcular pontos** | Quando ativado, o módulo atualiza dinamicamente os pontos exibidos na página do produto de acordo com as opções selecionadas. Os valores das opções podem possuir configurações próprias de pontos no OpenCart. |
| **Animação de contagem** | Anima a alteração numérica do preço durante as atualizações. Os números são animados durante a transição em vez de simplesmente serem substituídos. Esta opção é exclusivamente visual e pode ser utilizada para proporcionar uma transição mais suave entre os valores. |
| **Efeito de opacidade (Fade)** | Aplica uma transição visual de opacidade enquanto o preço está sendo atualizado. O efeito ajuda a indicar visualmente que o valor está sendo atualizado após uma alteração nas opções ou na quantidade.<br>**Importante:** quando a **Animação de contagem** está ativada, o módulo prioriza a animação numérica do preço em vez do efeito de opacidade.|
| **Status** | Ativa ou desativa o módulo. |

---

# Utilização na página do produto

Depois que o módulo estiver instalado, ativo e configurado, nenhuma ação adicional é necessária.

Ao acessar uma página de produto, o preço é calculado automaticamente.

---

# Compatibilidade com temas

O módulo atualiza os elementos de preço existentes na página do produto e trabalha com a estrutura padrão do catálogo do OpenCart.

Como temas de terceiros podem modificar a estrutura HTML da página do produto, a apresentação visual pode variar de acordo com o tema utilizado.

> **Importante:** o funcionamento dos cálculos é independente da aparência do tema. Caso um tema altere significativamente a estrutura padrão da página de produto, poderá ser necessária uma adaptação específica para esse tema. Se necessário, entre com contato com o suporte.

---

# Solução de problemas

## O preço não é atualizado

Verifique:

1. Se o módulo está instalado.
2. Se o módulo está com **Situação = Ativado**.
3. Se a extensão está habilitada no OpenCart.
4. Se as modificações foram atualizadas após a instalação.
5. Se o cache do OpenCart foi atualizado.
6. Se o cache do tema foi atualizado, quando aplicável.
7. Se a opção do produto possui uma alteração de preço configurada.

---

## O preço da opção não aparece corretamente

Verifique a configuração da opção diretamente no cadastro do produto.

Confirme:

- Valor da opção.
- Prefixo do preço.
- Produto associado à opção.
- Opção selecionada na página do produto.

O **Live Option Price** utiliza as informações cadastradas no OpenCart para realizar o cálculo.

---

## O preço não muda ao alterar a quantidade

Verifique se: **Multiplicar pela quantidade** está ativado nas configurações do módulo. Também confirme se o tema utiliza corretamente o campo de quantidade padrão do OpenCart.

---

## O desconto por quantidade não aparece

Confirme se existe uma regra de desconto cadastrada para:

- o produto;
- o grupo de clientes;
- a quantidade selecionada;
- o período atual.

Também verifique a prioridade das regras de desconto configuradas no OpenCart.

---

## O selo de desconto não aparece

Confirme se: **Exibir selo de desconto** está ativado. O selo somente é exibido quando existe uma porcentagem de desconto aplicável.

---

## O preço unitário não aparece

Confirme se: **Exibir preço unitário** está ativado. Também é necessário que o cálculo esteja considerando a quantidade e que a quantidade selecionada seja superior a uma unidade.

---

# Limpeza de cache

Depois de instalar ou atualizar o módulo, recomenda-se atualizar os caches do OpenCart.
Acesse: **Extensões > Modificações** e clique em:**Atualizar / Refresh** Também limpe o cache do tema, quando essa função estiver disponível na sua instalação.

> **Dica:** se uma alteração realizada no módulo não aparecer imediatamente, a primeira etapa de diagnóstico deve ser a limpeza dos caches.

---

## Desinstalação

Siga os passos abaixo para realizar uma desinstalação limpa e segura:

1. **Desinstalar**: Acesse **Extensions > Extensions**, filtre por **Modules**, localize o módulo e clique em **Uninstall**.
2. **Excluir**: Localize o módulo na lista de extensões instaladas e clique no ícone **Delete**.

> **O que acontece com os dados?**: A desinstalação remove somente as configurações e os arquivos do módulo.

---

# Suporte

Se você encontrar qualquer problema durante a instalação ou utilização do **Live Option Price**, utilize a página oficial da extensão no OpenCart Marketplace.

### Antes de solicitar suporte

Para facilitar o diagnóstico, informe:

- Versão do OpenCart.
- Versão do PHP.
- Tema utilizado.
- Versão do Live Option Price.
- Descrição do problema.
- Etapas necessárias para reproduzir o problema.

Sempre que possível, inclua capturas de tela das configurações e da página do produto.

### Obter suporte

[Obter suporte através do OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## Gostando do módulo?

Se o **Live Option Price** está ajudando sua loja e melhorando a experiência dos seus clientes, considere oferecer um café ao autor.

Isso ajuda a manter o desenvolvimento, a manutenção e as futuras atualizações do projeto.

[![Buy me a coffee](./assets/images/pt-br/buy_me_a_coffee.png)](https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW)

---

## Informações sobre a licença

Esta extensão é licenciada sob a **GNU General Public License v3.0 (GPL-3.0)**.

- O uso e a modificação do software devem estar de acordo com os termos estabelecidos pela licença GPL-3.0.
- O suporte técnico e as atualizações são fornecidos exclusivamente aos compradores originais através do OpenCart Marketplace oficial.
- Para obter todos os detalhes da licença, consulte o arquivo **LICENSE** distribuído com a extensão ou visite a página oficial da [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).

---

© 2026 **Rodrigoab** · [OpenCart Extensions](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)
