---
title: Компонент Person Card в наборе инструментов Microsoft Graph
description: Компонент Person-Card является компонентом для отображения дополнительных сведений, относящихся к пользователю.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 3d440f1340f9ee3f40c37538b1befcacd9867dc1
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144291"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="9198f-103">Компонент Person Card в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9198f-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9198f-104">Компонент Person-Card — это реагирующий на работу компонент для отображения дополнительных сведений, относящихся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="9198f-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="9198f-105">Он обычно используется в качестве всплывающего элемента в `mgt-person` компоненте.</span><span class="sxs-lookup"><span data-stu-id="9198f-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="9198f-106">Дополнительную информацию о компоненте `mgt-person` можно узнать в статье [упр](./person.md).</span><span class="sxs-lookup"><span data-stu-id="9198f-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="9198f-107">Пример</span><span class="sxs-lookup"><span data-stu-id="9198f-107">Example</span></span>

<span data-ttu-id="9198f-108">В следующем примере показано использование `mgt-person-card` компонента с `mgt-person` компонентом.</span><span class="sxs-lookup"><span data-stu-id="9198f-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="9198f-109">Наведите указатель мыши на лицо, чтобы увидеть карточку сотрудника, и используйте редактор кода, чтобы увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="9198f-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="9198f-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="9198f-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="9198f-111">Настройка интеграции с Teams</span><span class="sxs-lookup"><span data-stu-id="9198f-111">Setup for Teams integrations</span></span>

<span data-ttu-id="9198f-112">Компонент Person Card позволяет пользователю обращаться к конечному человеку, в том числе через чат Teams.</span><span class="sxs-lookup"><span data-stu-id="9198f-112">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="9198f-113">Если вы используете компонент в приложении "Вкладка Teams", вы можете убедиться, что компонент детально передается непосредственно в чат, а не открывает `microsoftTeamsLib` окно `TeamsProvider`браузера, задав значение in.</span><span class="sxs-lookup"><span data-stu-id="9198f-113">If using the component inside a Teams tab app, you can ensure that the component deep links directly to chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="9198f-114">Если компоненту Person Card не удается обнаружить lib Teams, компонент будет пытаться открыть веб-клиент Teams.</span><span class="sxs-lookup"><span data-stu-id="9198f-114">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

<span data-ttu-id="9198f-115">Для получения дополнительных сведений о `TeamsProvider` поставщике обратитесь к разделу [поставщик Microsoft Teams](../providers/teams.md).</span><span class="sxs-lookup"><span data-stu-id="9198f-115">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9198f-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="9198f-116">Properties</span></span>

<span data-ttu-id="9198f-117">Компонент использует Microsoft Graph для предоставления дополнительных сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="9198f-117">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="9198f-118">Чтобы определить пользователя, необходимо использовать свойство **Person — запрос** `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="9198f-118">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="9198f-119">Атрибут</span><span class="sxs-lookup"><span data-stu-id="9198f-119">Attribute</span></span>         | <span data-ttu-id="9198f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9198f-120">Type</span></span>                     | <span data-ttu-id="9198f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9198f-121">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="9198f-122">Person — сведения</span><span class="sxs-lookup"><span data-stu-id="9198f-122">person-details</span></span> | <span data-ttu-id="9198f-123">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="9198f-123">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="9198f-124">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="9198f-124">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="9198f-125">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="9198f-125">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="9198f-126">Объект Person, определенный Microsoft Graph, содержащий сведения, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="9198f-126">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="9198f-127">Person — изображение</span><span class="sxs-lookup"><span data-stu-id="9198f-127">person-image</span></span>   | <span data-ttu-id="9198f-128">PNG/JPG/SVG</span><span class="sxs-lookup"><span data-stu-id="9198f-128">png/jpg/svg</span></span>                    | <span data-ttu-id="9198f-129">Изображение, связанное с лицом, которое отображается в карточке.</span><span class="sxs-lookup"><span data-stu-id="9198f-129">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="9198f-130">inherit — Details</span><span class="sxs-lookup"><span data-stu-id="9198f-130">inherit-details</span></span>   | <span data-ttu-id="9198f-131">Нет.</span><span class="sxs-lookup"><span data-stu-id="9198f-131">None.</span></span>                  | <span data-ttu-id="9198f-132">Позволяет пользователю просматривать родительское дерево по родительскому `mgt-person` дереву, чтобы компонент `person-details` использовал `person-image` то же и данные.</span><span class="sxs-lookup"><span data-stu-id="9198f-132">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="9198f-133">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="9198f-133">Templates</span></span>

<span data-ttu-id="9198f-134">Компонент Person Card использует [шаблоны](../templates.md) , позволяющие добавлять или заменять части компонента.</span><span class="sxs-lookup"><span data-stu-id="9198f-134">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="9198f-135">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="9198f-135">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="9198f-136">Тип данных</span><span class="sxs-lookup"><span data-stu-id="9198f-136">Data type</span></span> | <span data-ttu-id="9198f-137">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="9198f-137">Data context</span></span> | <span data-ttu-id="9198f-138">Описание</span><span class="sxs-lookup"><span data-stu-id="9198f-138">Description</span></span> |
| - | - | - |
| <span data-ttu-id="9198f-139">нет данных</span><span class="sxs-lookup"><span data-stu-id="9198f-139">no-data</span></span> | <span data-ttu-id="9198f-140">null</span><span class="sxs-lookup"><span data-stu-id="9198f-140">null</span></span> | <span data-ttu-id="9198f-141">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="9198f-141">The template used when no data is available.</span></span>
| <span data-ttu-id="9198f-142">умолчани</span><span class="sxs-lookup"><span data-stu-id="9198f-142">default</span></span> | <span data-ttu-id="9198f-143">`person`: Объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="9198f-143">`person`: The person details object</span></span> <br> <span data-ttu-id="9198f-144">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="9198f-144">`personImage`: The URL of the image</span></span> | <span data-ttu-id="9198f-145">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="9198f-145">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="9198f-146">Person — сведения</span><span class="sxs-lookup"><span data-stu-id="9198f-146">person-details</span></span> | <span data-ttu-id="9198f-147">`person`: Объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="9198f-147">`person`: The person details object</span></span> | <span data-ttu-id="9198f-148">Шаблон, используемый для отображения верхней части карточки Person.</span><span class="sxs-lookup"><span data-stu-id="9198f-148">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="9198f-149">Contact — сведения</span><span class="sxs-lookup"><span data-stu-id="9198f-149">contact-details</span></span> | <span data-ttu-id="9198f-150">`person`: Объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="9198f-150">`person`: The person details object</span></span> | <span data-ttu-id="9198f-151">Шаблон, используемый для переопределения части сведений о контакте для контейнера дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="9198f-151">The template used to override the contact details part of the additional details container.</span></span> |
| <span data-ttu-id="9198f-152">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="9198f-152">additional-details</span></span> | <span data-ttu-id="9198f-153">`person`: Объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="9198f-153">`person`: The person details object</span></span> <br> <span data-ttu-id="9198f-154">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="9198f-154">`personImage`: the URL of the image</span></span> | <span data-ttu-id="9198f-155">Шаблон, используемый для добавления настраиваемого контента в контейнер дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="9198f-155">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="9198f-156">Например, вы можете использовать шаблон для настройки компонента, присоединенного к `mgt-person` компоненту, и шаблона, чтобы добавить дополнительные сведения в карточку.</span><span class="sxs-lookup"><span data-stu-id="9198f-156">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card inherit-details>
          <template data-type="additional-details">
            <h3>Stuffed Animal Friends:</h3>
            <ul>
              <li>Giraffe</li>
              <li>lion</li>
              <li>Rabbit</li>
            </ul>
          </template>
        </mgt-person-card>
      </template>
    </mgt-person>

```

## <a name="css-custom-properties"></a><span data-ttu-id="9198f-157">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="9198f-157">CSS custom properties</span></span>

<span data-ttu-id="9198f-158">`mgt-person-card` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="9198f-158">The `mgt-person-card` component defines the following CSS custom properties.</span></span> <span data-ttu-id="9198f-159">Чтобы использовать эти свойства, необходимо определить селектор в качестве родительского `mgt-person` элемента.</span><span class="sxs-lookup"><span data-stu-id="9198f-159">To use these properties, you must define the selector as the parent `mgt-person` element.</span></span> 

```css
mgt-person {
  --person-card-display-name-font-size: 40px;
  --person-card-display-name-color: #ffffff;
  --person-card-title-font-size: 20px;
  --person-card-title-color: #ffffff;
  --person-card-subtitle-font-size: 10px;
  --person-card-subtitle-color: #ffffff;
  --person-card-details-title-font-size: 10px;
  --person-card-details-title-color: #b3bf0a;
  --person-card-details-item-font-size: 20px;
  --person-card-details-item-color: #3abf0a;
  --person-card-background-color: #000000;
}
```

<span data-ttu-id="9198f-160">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="9198f-160">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="9198f-161">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9198f-161">Microsoft Graph permissions</span></span>

<span data-ttu-id="9198f-162">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений.</span><span class="sxs-lookup"><span data-stu-id="9198f-162">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="9198f-163">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="9198f-163">Authentication</span></span>

<span data-ttu-id="9198f-164">В элементе управления Person Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="9198f-164">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

## <a name="extend-for-more-control"></a><span data-ttu-id="9198f-165">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="9198f-165">Extend for more control</span></span>

<span data-ttu-id="9198f-166">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет `protected render*` несколько способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="9198f-166">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="9198f-167">Метод</span><span class="sxs-lookup"><span data-stu-id="9198f-167">Method</span></span> | <span data-ttu-id="9198f-168">Описание</span><span class="sxs-lookup"><span data-stu-id="9198f-168">Description</span></span> |
| - | - |
| <span data-ttu-id="9198f-169">рендернодата</span><span class="sxs-lookup"><span data-stu-id="9198f-169">renderNoData</span></span> | <span data-ttu-id="9198f-170">Отображает состояние, если данные о пользователях недоступны.</span><span class="sxs-lookup"><span data-stu-id="9198f-170">Renders a state when no person data is available.</span></span> | 
| <span data-ttu-id="9198f-171">рендерперсондетаилс</span><span class="sxs-lookup"><span data-stu-id="9198f-171">renderPersonDetails</span></span> | <span data-ttu-id="9198f-172">Отрисовывает основной текст карточки пользователя (изображение, имя, значки).</span><span class="sxs-lookup"><span data-stu-id="9198f-172">Renders the main body of the person card (image, name, icons).</span></span> |
| <span data-ttu-id="9198f-173">рендерперсонимаже</span><span class="sxs-lookup"><span data-stu-id="9198f-173">renderPersonImage</span></span> | <span data-ttu-id="9198f-174">Отрисовывает часть изображения сведений о лице.</span><span class="sxs-lookup"><span data-stu-id="9198f-174">Renders the image part of the person details.</span></span> |
| <span data-ttu-id="9198f-175">рендерперсоннаме</span><span class="sxs-lookup"><span data-stu-id="9198f-175">renderPersonName</span></span> | <span data-ttu-id="9198f-176">Отрисовывает часть имени сведений о лице.</span><span class="sxs-lookup"><span data-stu-id="9198f-176">Renders the name part of the person details.</span></span> |
| <span data-ttu-id="9198f-177">рендерперсонтитле</span><span class="sxs-lookup"><span data-stu-id="9198f-177">renderPersonTitle</span></span> | <span data-ttu-id="9198f-178">Отрисовывает часть заголовка сведений о лице.</span><span class="sxs-lookup"><span data-stu-id="9198f-178">Renders the title part of the person details.</span></span> |
| <span data-ttu-id="9198f-179">рендерперсонсубтитле</span><span class="sxs-lookup"><span data-stu-id="9198f-179">renderPersonSubtitle</span></span> | <span data-ttu-id="9198f-180">Отрисовывает часть сведений о лице в подзаголовках.</span><span class="sxs-lookup"><span data-stu-id="9198f-180">Renders the subtitle part of the person details.</span></span> |
| <span data-ttu-id="9198f-181">рендерконтактиконс</span><span class="sxs-lookup"><span data-stu-id="9198f-181">renderContactIcons</span></span> | <span data-ttu-id="9198f-182">Отрисовывает значки контактов, которые входят в сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="9198f-182">Renders the contact icons part of the person details.</span></span> |
| <span data-ttu-id="9198f-183">рендерекспандеддетаилсбуттон</span><span class="sxs-lookup"><span data-stu-id="9198f-183">renderExpandedDetailsButton</span></span> | <span data-ttu-id="9198f-184">Отрисовывает кнопку, чтобы Показать расширенные сведения.</span><span class="sxs-lookup"><span data-stu-id="9198f-184">Renders the button to show the expanded details.</span></span> |
| <span data-ttu-id="9198f-185">рендерекспандеддетаилс</span><span class="sxs-lookup"><span data-stu-id="9198f-185">renderExpandedDetails</span></span> | <span data-ttu-id="9198f-186">Отрисовывает содержимое в контейнере расширенных сведений.</span><span class="sxs-lookup"><span data-stu-id="9198f-186">Renders the content in the expanded details container.</span></span> |
| <span data-ttu-id="9198f-187">рендерконтактдетаилс</span><span class="sxs-lookup"><span data-stu-id="9198f-187">renderContactDetails</span></span> | <span data-ttu-id="9198f-188">Отрисовывает часть расширенных сведений о контакте.</span><span class="sxs-lookup"><span data-stu-id="9198f-188">Renders the contact details part of the expanded details.</span></span> |
| <span data-ttu-id="9198f-189">рендераддитионалдетаилс</span><span class="sxs-lookup"><span data-stu-id="9198f-189">renderAdditionalDetails</span></span> | <span data-ttu-id="9198f-190">Отрисовывает дополнительную информацию в части расширенных сведений.</span><span class="sxs-lookup"><span data-stu-id="9198f-190">Renders the additional details part of the expanded details.</span></span> |

