---
title: Person-Card компонента в microsoft Graph набор средств
description: Компонент Person-Card является компонентом для отображения дополнительных сведений, связанных с человеком.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 79a14c3d37fba06a076e319b34029008b7fbf2fd
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659185"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="2d545-103">Person-Card компонента в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="2d545-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="2d545-104">Компонент Person-Card — это адаптивный компонент для отображения дополнительных сведений, связанных с человеком.</span><span class="sxs-lookup"><span data-stu-id="2d545-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="2d545-105">Как правило, он используется в качестве flyout на `mgt-person` компоненте.</span><span class="sxs-lookup"><span data-stu-id="2d545-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="2d545-106">Дополнительные сведения о `mgt-person` компоненте см. [в mgt-person.](./person.md)</span><span class="sxs-lookup"><span data-stu-id="2d545-106">For more information about the `mgt-person` component, see [mgt-person](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="2d545-107">Пример</span><span class="sxs-lookup"><span data-stu-id="2d545-107">Example</span></span>

<span data-ttu-id="2d545-108">В следующем примере показано использование `mgt-person-card` компонента с `mgt-person` компонентом.</span><span class="sxs-lookup"><span data-stu-id="2d545-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="2d545-109">Наведите курсор на человека, чтобы увидеть карточку [](#properties) человека, и используйте редактор кода, чтобы увидеть, как свойства изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="2d545-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="2d545-110">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="2d545-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)


## <a name="global-component-configuration"></a><span data-ttu-id="2d545-111">Глобальная конфигурация компонентов</span><span class="sxs-lookup"><span data-stu-id="2d545-111">Global component configuration</span></span>

<span data-ttu-id="2d545-112">Класс `MgtPersonCard` предоставляет статический `config` объект, который настраивает все компоненты карточки человека в приложении.</span><span class="sxs-lookup"><span data-stu-id="2d545-112">The `MgtPersonCard` class exposes a static `config` object that configures all person card components in the application.</span></span> <span data-ttu-id="2d545-113">Объект config настраивает разделы и интерфейсы API, используемые карточкой пользователя для получения сведений о пользователе из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2d545-113">The config object configures what sections and what APIs are used by the person card to fetch details about a user from Microsoft Graph.</span></span>

<span data-ttu-id="2d545-114">По умолчанию все разделы и API включены.</span><span class="sxs-lookup"><span data-stu-id="2d545-114">By default, all sections and APIs are enabled.</span></span> <span data-ttu-id="2d545-115">В следующем примере показано, как использовать объект config для отключения разделов или API.</span><span class="sxs-lookup"><span data-stu-id="2d545-115">The following example shows how to use the config object to disable sections or APIs.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

<span data-ttu-id="2d545-116">Для объекта config доступны следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="2d545-116">The following properties are available on the config object.</span></span>

| <span data-ttu-id="2d545-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d545-117">Property</span></span> | <span data-ttu-id="2d545-118">Описание</span><span class="sxs-lookup"><span data-stu-id="2d545-118">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="2d545-119">useContactApis</span><span class="sxs-lookup"><span data-stu-id="2d545-119">useContactApis</span></span> | <span data-ttu-id="2d545-120">`boolean` - Указывает, может ли компонент карточки человека использовать API контактов Microsoft Graph для поиска контактных данных и фотографий.</span><span class="sxs-lookup"><span data-stu-id="2d545-120">`boolean` - Indicates whether the person card component can use the Microsoft Graph Contact API to search for contact details and photos.</span></span> <span data-ttu-id="2d545-121">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="2d545-121">Default value is `true`.</span></span>  |
| <span data-ttu-id="2d545-122">sections</span><span class="sxs-lookup"><span data-stu-id="2d545-122">sections</span></span> | <span data-ttu-id="2d545-123">`object` - Настраивает разделы, которые будут показаны в карточке человека.</span><span class="sxs-lookup"><span data-stu-id="2d545-123">`object` - Configures what sections are shown in the person card.</span></span>  |

### <a name="person-card-sections"></a><span data-ttu-id="2d545-124">Разделы карточки человека</span><span class="sxs-lookup"><span data-stu-id="2d545-124">Person card sections</span></span>

<span data-ttu-id="2d545-125">Карточка человека содержит несколько настраиваемых разделов для отображения сведений о человеке:</span><span class="sxs-lookup"><span data-stu-id="2d545-125">The person card contains several configurable sections for displaying person details:</span></span>
* <span data-ttu-id="2d545-126">Contact - Contact information such as email, phone, position, location, and more.</span><span class="sxs-lookup"><span data-stu-id="2d545-126">Contact - Contact information such as email, phone, position, location, and more.</span></span>
* <span data-ttu-id="2d545-127">Организация — организационный график с руководителями, прямыми отчетами и соответствующими людьми.</span><span class="sxs-lookup"><span data-stu-id="2d545-127">Organization - Organizational graph with managers, direct reports, and relevant people.</span></span>
* <span data-ttu-id="2d545-128">Сообщения — наиболее релевантные сообщения электронной почты с текущим во время вписаного пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d545-128">Messages - Most relevant email messages with the current signed in user.</span></span>
* <span data-ttu-id="2d545-129">Файлы — наиболее релевантные общие файлы для текущего пользователя, выписав его.</span><span class="sxs-lookup"><span data-stu-id="2d545-129">Files - Most relevant shared files with the current signed in user.</span></span>
* <span data-ttu-id="2d545-130">Профиль — сведения профиля, такие как проекты, навыки, языки и другие.</span><span class="sxs-lookup"><span data-stu-id="2d545-130">Profile - Profile information such as projects, skills, languages, and more.</span></span>

<span data-ttu-id="2d545-131">Разделы загружаются по умолчанию, но их можно отключить глобально с помощью `MgtPersonCard.config.sections` свойства объекта.</span><span class="sxs-lookup"><span data-stu-id="2d545-131">Sections are loaded by default, but they can be disabled globally via the `MgtPersonCard.config.sections` object property.</span></span> <span data-ttu-id="2d545-132">Доступны следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="2d545-132">The following properties are available.</span></span>

| <span data-ttu-id="2d545-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d545-133">Property</span></span> | <span data-ttu-id="2d545-134">Описание</span><span class="sxs-lookup"><span data-stu-id="2d545-134">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="2d545-135">organization;</span><span class="sxs-lookup"><span data-stu-id="2d545-135">organization</span></span> | <span data-ttu-id="2d545-136">`boolean` - Указывает, отображается ли раздел организации карточки человека.</span><span class="sxs-lookup"><span data-stu-id="2d545-136">`boolean` - Indicates whether the person card organization section is shown.</span></span> <span data-ttu-id="2d545-137">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="2d545-137">Default value is `true`.</span></span>  |
| <span data-ttu-id="2d545-138">mailMessages</span><span class="sxs-lookup"><span data-stu-id="2d545-138">mailMessages</span></span> | <span data-ttu-id="2d545-139">`boolean` - Указывает, отображается ли раздел сообщений карточки человека.</span><span class="sxs-lookup"><span data-stu-id="2d545-139">`boolean` - Indicates whether the person card messages section is shown.</span></span> <span data-ttu-id="2d545-140">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="2d545-140">Default value is `true`.</span></span>  |
| <span data-ttu-id="2d545-141">files</span><span class="sxs-lookup"><span data-stu-id="2d545-141">files</span></span> | <span data-ttu-id="2d545-142">`boolean` - Указывает, отображается ли раздел "Файлы карточки человека".</span><span class="sxs-lookup"><span data-stu-id="2d545-142">`boolean` - Indicates whether the person card files section is shown.</span></span> <span data-ttu-id="2d545-143">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="2d545-143">Default value is `true`.</span></span>  |
| <span data-ttu-id="2d545-144">profile</span><span class="sxs-lookup"><span data-stu-id="2d545-144">profile</span></span> | <span data-ttu-id="2d545-145">`boolean` - Указывает, отображается ли раздел профиля карточки пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d545-145">`boolean` - Indicates whether the person card profile section is shown.</span></span> <span data-ttu-id="2d545-146">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="2d545-146">Default value is `true`.</span></span>  |

<span data-ttu-id="2d545-147">Чтобы отключить раздел, просто задайте свойство в коде инициализации `false` приложения:.</span><span class="sxs-lookup"><span data-stu-id="2d545-147">To disable a section, simply set the property to `false` in your app initialization code:.</span></span>
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="2d545-148">Настройка интеграции Teams</span><span class="sxs-lookup"><span data-stu-id="2d545-148">Setup for Teams integrations</span></span>

<span data-ttu-id="2d545-149">Компонент Person-Card позволяет пользователю связаться с целевым пользователем, в том числе с помощью чата Teams.</span><span class="sxs-lookup"><span data-stu-id="2d545-149">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="2d545-150">Если компонент используется в приложении для вкладки Teams, можно убедиться, что компонент имеет прямую ссылку непосредственно на чат, а не открывает окно браузера, задав `microsoftTeamsLib` `TeamsProvider` его.</span><span class="sxs-lookup"><span data-stu-id="2d545-150">If using the component inside a Teams tab app, you can ensure that the component deep links directly to a chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="2d545-151">Если Person-Card не удается обнаружить lib Teams, он попытается открыть веб-клиент Teams.</span><span class="sxs-lookup"><span data-stu-id="2d545-151">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as MicrosoftTeams from "@microsoft/teams-js/dist/MicrosoftTeams";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = MicrosoftTeams;
```

<span data-ttu-id="2d545-152">Дополнительные сведения о `TeamsProvider` поставщике см. в [сведениях о поставщике Microsoft Teams.](../providers/teams.md)</span><span class="sxs-lookup"><span data-stu-id="2d545-152">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2d545-153">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d545-153">Properties</span></span>

<span data-ttu-id="2d545-154">По умолчанию компонент передает сведения о `mgt-person` человеке `mgt-person-card` компоненту.</span><span class="sxs-lookup"><span data-stu-id="2d545-154">By default, the `mgt-person` component will pass the person details to the `mgt-person-card` component.</span></span> <span data-ttu-id="2d545-155">Однако эти атрибуты можно использовать для изменения этого шаблона компонента или при использовании компонента в качестве `mgt-person` `mgt-person-card` автономного компонента.</span><span class="sxs-lookup"><span data-stu-id="2d545-155">However, you can use these attributes to change this when templating the `mgt-person` component or when using the `mgt-person-card` component as a standalone component.</span></span>

| <span data-ttu-id="2d545-156">Атрибут</span><span class="sxs-lookup"><span data-stu-id="2d545-156">Attribute</span></span>         | <span data-ttu-id="2d545-157">Тип</span><span class="sxs-lookup"><span data-stu-id="2d545-157">Type</span></span>                     | <span data-ttu-id="2d545-158">Описание</span><span class="sxs-lookup"><span data-stu-id="2d545-158">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="2d545-159">person-details</span><span class="sxs-lookup"><span data-stu-id="2d545-159">person-details</span></span> | <span data-ttu-id="2d545-160">MicrosoftGraph.User</span><span class="sxs-lookup"><span data-stu-id="2d545-160">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="2d545-161">MicrosoftGraph.Person</span><span class="sxs-lookup"><span data-stu-id="2d545-161">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="2d545-162">MicrosoftGraph.Contact</span><span class="sxs-lookup"><span data-stu-id="2d545-162">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="2d545-163">Объект Person, определенный в Microsoft Graph, содержащий сведения, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="2d545-163">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="2d545-164">person-image</span><span class="sxs-lookup"><span data-stu-id="2d545-164">person-image</span></span>   | <span data-ttu-id="2d545-165">Строка</span><span class="sxs-lookup"><span data-stu-id="2d545-165">string</span></span>                    | <span data-ttu-id="2d545-166">URI изображения, связанного с человеком, отображаемого на карточке.</span><span class="sxs-lookup"><span data-stu-id="2d545-166">Image uri related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="2d545-167">inherit-details</span><span class="sxs-lookup"><span data-stu-id="2d545-167">inherit-details</span></span>   | <span data-ttu-id="2d545-168">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d545-168">None.</span></span>                  | <span data-ttu-id="2d545-169">Позволяет карточке человека походить по родительскому дереву, чтобы компонент использует `mgt-person` те же данные и `person-details` `person-image` данные.</span><span class="sxs-lookup"><span data-stu-id="2d545-169">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |
| <span data-ttu-id="2d545-170">user-id</span><span class="sxs-lookup"><span data-stu-id="2d545-170">user-id</span></span> | <span data-ttu-id="2d545-171">Строка</span><span class="sxs-lookup"><span data-stu-id="2d545-171">string</span></span> | <span data-ttu-id="2d545-172">Позволяет разработчикам предоставить удостоверение пользователя для ирисовки данных, показанных в компоненте карточки пользователя</span><span class="sxs-lookup"><span data-stu-id="2d545-172">Allows developers to supply user-id to retrive data shown on person-card component</span></span> |
| <span data-ttu-id="2d545-173">person-query</span><span class="sxs-lookup"><span data-stu-id="2d545-173">person-query</span></span> | <span data-ttu-id="2d545-174">Строка</span><span class="sxs-lookup"><span data-stu-id="2d545-174">string</span></span> | <span data-ttu-id="2d545-175">Позволяет разработчикам запрашивать данные, показанные в компоненте карточки пользователя</span><span class="sxs-lookup"><span data-stu-id="2d545-175">Allows developers to supply person-query to retrive data shown on person-card component</span></span> |


## <a name="templates"></a><span data-ttu-id="2d545-176">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="2d545-176">Templates</span></span>

<span data-ttu-id="2d545-177">Компонент Person-Card использует [шаблоны,](../customize-components/templates.md) позволяющие добавлять или заменять части компонента.</span><span class="sxs-lookup"><span data-stu-id="2d545-177">The Person-Card component uses [templates](../customize-components/templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="2d545-178">Чтобы указать шаблон, включив элемент внутри компонента, закажите одно из `<template>` `data-type` следующих значений.</span><span class="sxs-lookup"><span data-stu-id="2d545-178">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="2d545-179">Тип данных</span><span class="sxs-lookup"><span data-stu-id="2d545-179">Data type</span></span> | <span data-ttu-id="2d545-180">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="2d545-180">Data context</span></span> | <span data-ttu-id="2d545-181">Описание</span><span class="sxs-lookup"><span data-stu-id="2d545-181">Description</span></span> |
| - | - | - |
| <span data-ttu-id="2d545-182">no-data</span><span class="sxs-lookup"><span data-stu-id="2d545-182">no-data</span></span> | <span data-ttu-id="2d545-183">null</span><span class="sxs-lookup"><span data-stu-id="2d545-183">null</span></span> | <span data-ttu-id="2d545-184">Шаблон, используемый, когда данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="2d545-184">The template used when no data is available.</span></span>
| <span data-ttu-id="2d545-185">default</span><span class="sxs-lookup"><span data-stu-id="2d545-185">default</span></span> | <span data-ttu-id="2d545-186">`person`: объект сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="2d545-186">`person`: The person details object</span></span> <br> <span data-ttu-id="2d545-187">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="2d545-187">`personImage`: The URL of the image</span></span> | <span data-ttu-id="2d545-188">Шаблон по умолчанию заменяет весь компонент на собственный.</span><span class="sxs-lookup"><span data-stu-id="2d545-188">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="2d545-189">person-details</span><span class="sxs-lookup"><span data-stu-id="2d545-189">person-details</span></span> | <span data-ttu-id="2d545-190">`person`: объект сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="2d545-190">`person`: The person details object</span></span> | <span data-ttu-id="2d545-191">Шаблон, используемый для отображения верхней части карточки человека.</span><span class="sxs-lookup"><span data-stu-id="2d545-191">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="2d545-192">additional-details</span><span class="sxs-lookup"><span data-stu-id="2d545-192">additional-details</span></span> | <span data-ttu-id="2d545-193">`person`: объект сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="2d545-193">`person`: The person details object</span></span> <br> <span data-ttu-id="2d545-194">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="2d545-194">`personImage`: the URL of the image</span></span> | <span data-ttu-id="2d545-195">Шаблон, используемый для добавления пользовательского содержимого в контейнер дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="2d545-195">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="2d545-196">Например, можно использовать шаблон для настройки компонента, подключенного к компоненту, и шаблон для добавления дополнительных сведений `mgt-person` в карточку.</span><span class="sxs-lookup"><span data-stu-id="2d545-196">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" view="twolines" person-card="hover">
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

## <a name="css-custom-properties"></a><span data-ttu-id="2d545-197">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="2d545-197">CSS custom properties</span></span>

<span data-ttu-id="2d545-198">Компонент `mgt-person-card` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="2d545-198">The `mgt-person-card` component defines the following CSS custom properties.</span></span> 

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

<span data-ttu-id="2d545-199">Дополнительные узнать см. [в компонентах стиля.](../customize-components/style.md)</span><span class="sxs-lookup"><span data-stu-id="2d545-199">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-apis-and-permissions"></a><span data-ttu-id="2d545-200">API и разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2d545-200">Microsoft Graph APIs and permissions</span></span>

<span data-ttu-id="2d545-201">В Person-Card используются следующие API Microsoft Graph и разрешения.</span><span class="sxs-lookup"><span data-stu-id="2d545-201">The Person-Card control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="2d545-202">Ресурс</span><span class="sxs-lookup"><span data-stu-id="2d545-202">Resource</span></span> | <span data-ttu-id="2d545-203">Разрешение</span><span class="sxs-lookup"><span data-stu-id="2d545-203">Permission</span></span> | <span data-ttu-id="2d545-204">Раздел</span><span class="sxs-lookup"><span data-stu-id="2d545-204">Section</span></span> |
| - | - | - |
| [<span data-ttu-id="2d545-205">/me</span><span class="sxs-lookup"><span data-stu-id="2d545-205">/me</span></span>](/graph/api/user-get) | <span data-ttu-id="2d545-206">User.Read</span><span class="sxs-lookup"><span data-stu-id="2d545-206">User.Read</span></span> | <span data-ttu-id="2d545-207">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="2d545-207">Default</span></span> |
| [<span data-ttu-id="2d545-208">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="2d545-208">/me/photo/$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="2d545-209">User.Read</span><span class="sxs-lookup"><span data-stu-id="2d545-209">User.Read</span></span> | <span data-ttu-id="2d545-210">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="2d545-210">Default</span></span> |
| [<span data-ttu-id="2d545-211">/me/people/?$search=</span><span class="sxs-lookup"><span data-stu-id="2d545-211">/me/people/?$search=</span></span>](/graph/api/user-list-people) | <span data-ttu-id="2d545-212">People.Read</span><span class="sxs-lookup"><span data-stu-id="2d545-212">People.Read</span></span> | <span data-ttu-id="2d545-213">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="2d545-213">Default</span></span> |
| [<span data-ttu-id="2d545-214">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="2d545-214">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="2d545-215">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="2d545-215">Contacts.Read</span></span> | <span data-ttu-id="2d545-216">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="2d545-216">Default</span></span> |
| [<span data-ttu-id="2d545-217">/users/{id}</span><span class="sxs-lookup"><span data-stu-id="2d545-217">/users/{id}</span></span>](/graph/api/user-list-people) | <span data-ttu-id="2d545-218">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="2d545-218">User.ReadBasic.All</span></span> | <span data-ttu-id="2d545-219">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="2d545-219">Default</span></span> |
| [<span data-ttu-id="2d545-220">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="2d545-220">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) | <span data-ttu-id="2d545-221">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="2d545-221">User.ReadBasic.All</span></span> | <span data-ttu-id="2d545-222">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="2d545-222">Default</span></span> |
| [<span data-ttu-id="2d545-223">/me/presence</span><span class="sxs-lookup"><span data-stu-id="2d545-223">/me/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="2d545-224">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="2d545-224">Presence.Read</span></span> | <span data-ttu-id="2d545-225">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="2d545-225">Default</span></span> |
| [<span data-ttu-id="2d545-226">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="2d545-226">/users/{id}/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="2d545-227">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d545-227">Presence.Read.All</span></span> | <span data-ttu-id="2d545-228">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="2d545-228">Default</span></span> |
| [<span data-ttu-id="2d545-229">/users/{id}/manager</span><span class="sxs-lookup"><span data-stu-id="2d545-229">/users/{id}/manager</span></span>](/graph/api/user-list-manager) | <span data-ttu-id="2d545-230">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d545-230">User.Read.All</span></span> | <span data-ttu-id="2d545-231">Организация</span><span class="sxs-lookup"><span data-stu-id="2d545-231">Organization</span></span> |
| [<span data-ttu-id="2d545-232">/users/{id}/directReports</span><span class="sxs-lookup"><span data-stu-id="2d545-232">/users/{id}/directReports</span></span>](/graph/api/user-list-directreports) | <span data-ttu-id="2d545-233">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d545-233">User.Read.All</span></span> | <span data-ttu-id="2d545-234">Организация</span><span class="sxs-lookup"><span data-stu-id="2d545-234">Organization</span></span> |
| [<span data-ttu-id="2d545-235">/users/{id}/people</span><span class="sxs-lookup"><span data-stu-id="2d545-235">/users/{id}/people</span></span>](/graph/api/user-list-people) | <span data-ttu-id="2d545-236">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d545-236">People.Read.All</span></span> | <span data-ttu-id="2d545-237">Организация</span><span class="sxs-lookup"><span data-stu-id="2d545-237">Organization</span></span> |
| [<span data-ttu-id="2d545-238">/me/messages</span><span class="sxs-lookup"><span data-stu-id="2d545-238">/me/messages</span></span>](/graph/api/user-list-messages) | <span data-ttu-id="2d545-239">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="2d545-239">Mail.ReadBasic</span></span> | <span data-ttu-id="2d545-240">Сообщения</span><span class="sxs-lookup"><span data-stu-id="2d545-240">Messages</span></span> |
| <span data-ttu-id="2d545-241">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span><span class="sxs-lookup"><span data-stu-id="2d545-241">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span></span> | <span data-ttu-id="2d545-242">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d545-242">Sites.Read.All</span></span> | <span data-ttu-id="2d545-243">Файлы</span><span class="sxs-lookup"><span data-stu-id="2d545-243">Files</span></span> |
| [<span data-ttu-id="2d545-244">/users/{id}/profile</span><span class="sxs-lookup"><span data-stu-id="2d545-244">/users/{id}/profile</span></span>](/graph/api/profile-get) | <span data-ttu-id="2d545-245">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="2d545-245">User.Read.All</span></span> | <span data-ttu-id="2d545-246">Профиль</span><span class="sxs-lookup"><span data-stu-id="2d545-246">Profile</span></span> |

<span data-ttu-id="2d545-247">Класс также предоставляет статический метод, который возвращает массив областей, необходимых для работы карточки человека на основе глобальной конфигурации `MgtPersonCard` `getScopes` карточки человека.</span><span class="sxs-lookup"><span data-stu-id="2d545-247">The `MgtPersonCard` class also exposes a `getScopes` static method that returns an array of scopes required for the person card to function based on the global person card configuration.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a><span data-ttu-id="2d545-248">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="2d545-248">Authentication</span></span>

<span data-ttu-id="2d545-249">В Person-Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="2d545-249">The Person-Card control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 
