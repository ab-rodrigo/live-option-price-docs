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

O **Live Option Price** atualiza o preço do produto em tempo real conforme o cliente seleciona as suas opções, altera a quantidade ou modifica outras informações relacionadas com o produto.

Sem o módulo, o preço exibido na página do produto pode permanecer inalterado até que o cliente conclua uma ação adicional. Com o **Live Option Price**, os valores são recalculados automaticamente e apresentados diretamente na página do produto.

O módulo utiliza os valores configurados nativamente no OpenCart, incluindo:

- Preço do produto.
- Preço das opções.
- Descontos.
- Preço especial.
- Impostos (Taxas).
- Pontos do produto e das opções, quando ativado.
- Quantidade selecionada.

O resultado é apresentado diretamente na página do produto, proporcionando ao cliente uma visualização imediata do valor correspondente à configuração escolhida.

### Compatibilidade

O **Live Option Price** foi desenvolvido para funcionar nas versões:

- **OpenCart 3.x**
- **OpenCart 4.x**

A interface de administração e o funcionamento podem apresentar pequenas diferenças visuais entre as versões do OpenCart, mas as funcionalidades e as configurações do módulo permanecem as mesmas.

---

## Requisitos

Certifique-se de que possui permissões de administração para:

- **Instalador de Extensões**
- **Extensões / Módulos**
- **Modificações**
- **Configuração do módulo**

> **Importante:** a instalação deve ser realizada utilizando o ficheiro oficial do módulo fornecido para a sua versão do OpenCart.

---

## Principais funcionalidades

| Funcionalidade | Descrição |
| :--- | :--- |
| **Preço em tempo real** | Atualiza o preço automaticamente quando o cliente altera as opções do produto. |
| **Preços das opções** | Considera os acréscimos e descontos definidos nas opções do produto. |
| **Descontos por quantidade** | Considera automaticamente os descontos por quantidade configurados no OpenCart. |
| **Preço especial** | Mantém o cálculo compatível com o preço especial do produto. |
| **Multiplicar pela quantidade** | Permite exibir o valor total de acordo com a quantidade selecionada. |
| **Preço unitário** | Exibe o preço correspondente a uma unidade quando o cliente seleciona mais de uma unidade. |
| **Selo de desconto** | Exibe visualmente a percentagem de desconto aplicada ao produto. |
| **Impostos** | Atualiza a informação de preço relacionada com os impostos conforme a configuração fiscal do OpenCart. |
| **Pontos** | Atualiza os pontos exibidos para o produto conforme as opções selecionadas e a quantidade. |
| **Animação de contagem** | Anima a alteração numérica do preço durante as atualizações. |
| **Efeito de opacidade (Fade)** | Aplica uma transição visual durante a atualização do preço. |

---

> **Importante:** o módulo não substitui a configuração de preços do OpenCart. Este utiliza os valores existentes no produto, nas opções, nos descontos e nas configurações fiscais da loja para realizar o cálculo.

---

## Instalação

Siga o fluxo abaixo para instalar o módulo:

1. **Download**: Obtenha o módulo oficial diretamente no [OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr).
2. **Upload**: No painel de administração da sua loja, aceda a **Extensões > Instalador**, clique em **Upload** e selecione o ficheiro descarregado.
3. **Ativação**: Localize o módulo na lista de extensões e clique no ícone **Instalar** para o ativar.

> **Dica técnica**: Após a ativação, lembre-se de aceder a **Extensões > Modificações** e clicar no botão **Atualizar (Refresh)** (ícone azul) para limpar a cache do sistema.

---

## Aceder às configurações

Depois de instalar o módulo:

1. Aceda a **Extensões > Extensões**.
2. Filtre por **Módulos**.
3. Localize **Live Option Price**.
4. Clique em **Editar**.

---

# Configurações

![Configuração](./assets/images/pt-br/docs-config-pt-br.png)

| Parâmetro | Função |
|---|---|
| **Multiplicar pela quantidade** | Determina se o preço exibido deverá considerar a quantidade selecionada pelo cliente.<br>**Importante:** esta configuração controla especificamente a forma como o preço é apresentado. A quantidade continua a ser considerada pelo OpenCart nas restantes operações aplicáveis. |
| **Exibir selo de desconto** | Exibe um selo com a percentagem de desconto quando o produto possui um preço promocional ou desconto por quantidade aplicável.<br>**Importante:** a percentagem apresentada é calculada pelo módulo com base na diferença entre o preço utilizado como referência e o preço com desconto aplicado. |
| **Exibir preço unitário** | Exibe o valor correspondente a uma unidade do produto quando a quantidade selecionada for superior a 1. O preço unitário é exibido quando o cálculo está configurado para considerar a quantidade e a quantidade selecionada é superior a uma unidade.<br>**Nota:** esta função apenas atualiza a informação apresentada dinamicamente na página do produto. As regras de pontos do OpenCart continuam a ser a fonte dos valores utilizados pelo módulo. |
| **Calcular pontos** | Quando ativado, o módulo atualiza dinamicamente os pontos exibidos na página do produto de acordo com as opções selecionadas. Os valores das opções podem possuir configurações próprias de pontos no OpenCart. |
| **Animação de contagem** | Anima a alteração numérica do preço durante as atualizações. Os números são animados durante a transição em vez de simplesmente serem substituídos. Esta opção é exclusivamente visual e pode ser utilizada para proporcionar uma transição mais suave entre os valores. |
| **Efeito de opacidade (Fade)** | Aplica uma transição visual de opacidade enquanto o preço está a ser atualizado. O efeito ajuda a indicar visualmente que o valor está a ser atualizado após uma alteração nas opções ou na quantidade.<br>**Importante:** quando a **Animação de contagem** está ativada, o módulo prioriza a animação numérica do preço em vez do efeito de opacidade.|
| **Estado** | Ativa ou desativa o módulo. |

---

# Utilização na página do produto

Depois de o módulo estar instalado, ativo e configurado, nenhuma ação adicional é necessária.

Ao aceder a uma página de produto, o preço é calculado automaticamente.

---

# Compatibilidade com temas

O módulo atualiza os elementos de preço existentes na página do produto e trabalha com a estrutura padrão do catálogo do OpenCart.

Como os temas de terceiros podem modificar a estrutura HTML da página do produto, a apresentação visual pode variar de acordo com o tema utilizado.

> **Importante:** o funcionamento dos cálculos é independente da aparência do tema. Caso um tema altere significativamente a estrutura padrão da página do produto, poderá ser necessária uma adaptação específica para esse tema. Se necessário, entre com contacto com o suporte.

---

# Resolução de problemas

## O preço não é atualizado

Verifique:

1. Se o módulo está instalado.
2. Se o módulo está com **Estado = Ativado**.
3. Se a extensão está ativada no OpenCart.
4. Se as modificações foram atualizadas após a instalação.
5. Se a cache do OpenCart foi atualizada.
6. Se a cache do tema foi atualizada, quando aplicável.
7. Se a opção do produto possui uma alteração de preço configurada.

---

## O preço da opção não aparece corretamente

Verifique a configuração da opção diretamente no registo do produto.

Confirme:

- Valor da opção.
- Prefixo do preço.
- Produto associado à opção.
- Opção selecionada na página do produto.

O **Live Option Price** utiliza as informações registadas no OpenCart para realizar o cálculo.

---

## O preço não muda ao alterar a quantidade

Verifique se: **Multiplicar pela quantidade** está ativado nas configurações do módulo. Confirme também se o tema utiliza corretamente o campo de quantidade padrão do OpenCart.

---

## O desconto por quantidade não aparece

Confirme se existe uma regra de desconto registada para:

- o produto;
- o grupo de clientes;
- a quantidade selecionada;
- o período atual.

Verifique também a prioridade das regras de desconto configuradas no OpenCart.

---

## O selo de desconto não aparece

Confirme se: **Exibir selo de desconto** está ativado. O selo apenas é exibido quando existe uma percentagem de desconto aplicável.

---

## O preço unitário não aparece

Confirme se: **Exibir preço unitário** está ativado. Também é necessário que o cálculo esteja a considerar a quantidade e que a quantidade selecionada seja superior a uma unidade.

---

# Limpeza de cache

Depois de instalar ou atualizar o módulo, recomenda-se atualizar as caches do OpenCart.
Aceda a: **Extensões > Modificações** e clique em: **Atualizar (Refresh)**. Limpe também a cache do tema, quando esta função estiver disponível na sua instalação.

> **Dica:** se uma alteração realizada no módulo não aparecer imediatamente, a primeira etapa de diagnóstico deve ser a limpeza das caches.

---

## Desinstalação

Siga os passos abaixo para realizar uma desinstalação limpa e segura:

1. **Desinstalar**: Aceda a **Extensões > Extensões**, filtre por **Módulos**, localize o módulo e clique em **Desinstalar (Uninstall)**.
2. **Eliminar**: Localize o módulo na lista de extensões instaladas e clique no ícone **Eliminar (Delete)**.

> **O que acontece aos dados?**: A desinstalação remove apenas as configurações e os ficheiros do módulo.

---

# Suporte

Se encontrar qualquer problema durante a instalação ou utilização do **Live Option Price**, utilize a página oficial da extensão no OpenCart Marketplace.

### Antes de solicitar suporte

Para facilitar o diagnóstico, informe:

- Versão do OpenCart.
- Versão do PHP.
- Tema utilizado.
- Versão do Live Option Price.
- Descrição do problema.
- Passos necessários para reproduzir o problema.

Sempre que possível, inclua capturas de ecrã das configurações e da página do produto.

### Obter suporte

[Obter suporte através do OpenCart Marketplace](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)

---

## A gostar do módulo?

Se o **Live Option Price** está a ajudar a sua loja e a melhorar a experiência dos seus clientes, considere oferecer um café ao autor.

Isto ajuda a manter o desenvolvimento, a manutenção e as futuras atualizações do projeto.

[![Buy me a coffee](./assets/images/pt-pt/buy_me_a_coffee.png)](https://www.paypal.com/donate/?hosted_button_id=SPQH2B32XBJUW)

---

## Informações sobre a licença

Esta extensão é licenciada sob a **GNU General Public License v3.0 (GPL-3.0)**.

- O uso e a modificação do software devem estar de acordo com os termos estabelecidos pela licença GPL-3.0.
- O suporte técnico e as atualizações são fornecidos exclusivamente aos compradores originais através do OpenCart Marketplace oficial.
- Para obter todos os detalhes da licença, consulte o ficheiro **LICENSE** distribuído com a extensão ou visite a página oficial da [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).

---

© 2026 **Rodrigoab** · [OpenCart Extensions](https://www.opencart.com/index.php?route=marketplace/extension&filter_member=Rodrigoabr)