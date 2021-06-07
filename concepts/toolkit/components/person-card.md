---
title: Компонент Person-Card в Microsoft Graph Toolkit
description: Компонент Person-Card для просмотра дополнительных сведений, относящихся к пользователю.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 8497dbb3b3d9a3173cdbf8ee8ec6bfe74859868b
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780703"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="16774-103">Компонент Person-Card в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="16774-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="16774-104">Компонент Person-Card — это адаптивный компонент для просмотра дополнительных сведений, относящихся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="16774-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="16774-105">Обычно используется в качестве всплывающего окна для компонента `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="16774-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="16774-106">Дополнительные сведения о компоненте `mgt-person` см. в разделе [mgt-person](./person.md).</span><span class="sxs-lookup"><span data-stu-id="16774-106">For more information about the `mgt-person` component, see [mgt-person](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="16774-107">Пример</span><span class="sxs-lookup"><span data-stu-id="16774-107">Example</span></span>

<span data-ttu-id="16774-108">В приведенном ниже примере показано использование компонента `mgt-person-card` с компонентом `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="16774-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="16774-109">Наведите указатель мыши на человека, чтобы увидеть карточку контакта, а затем в редакторе кода посмотрите, как [свойства](#properties) изменить поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="16774-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card&source=docs" height="400"></iframe>

[<span data-ttu-id="16774-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="16774-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card&source=docs)


## <a name="global-component-configuration"></a><span data-ttu-id="16774-111">Настройка глобального компонента</span><span class="sxs-lookup"><span data-stu-id="16774-111">Global component configuration</span></span>

<span data-ttu-id="16774-112">Класс `MgtPersonCard` предоставляет статический объект `config`, который конфигурирует все компоненты карточки контакта в приложении.</span><span class="sxs-lookup"><span data-stu-id="16774-112">The `MgtPersonCard` class exposes a static `config` object that configures all person card components in the application.</span></span> <span data-ttu-id="16774-113">В объекте config настраивается, какие разделы и какие API-интерфейсы используются для получения сведений о пользователе в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="16774-113">The config object configures what sections and what APIs are used by the person card to fetch details about a user from Microsoft Graph.</span></span>

<span data-ttu-id="16774-114">По умолчанию все разделы и API-интерфейсы включены.</span><span class="sxs-lookup"><span data-stu-id="16774-114">By default, all sections and APIs are enabled.</span></span> <span data-ttu-id="16774-115">В приведенном ниже примере показано, как использовать объект конфигурации для отключения разделов и API-интерфейсов.</span><span class="sxs-lookup"><span data-stu-id="16774-115">The following example shows how to use the config object to disable sections or APIs.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.useContactApis = false;
MgtPersonCard.config.sections.profile = false;
```

<span data-ttu-id="16774-116">Ниже указаны свойства, доступные в объекте конфигурации.</span><span class="sxs-lookup"><span data-stu-id="16774-116">The following properties are available on the config object.</span></span>

| <span data-ttu-id="16774-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="16774-117">Property</span></span> | <span data-ttu-id="16774-118">Описание</span><span class="sxs-lookup"><span data-stu-id="16774-118">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="16774-119">useContactApis</span><span class="sxs-lookup"><span data-stu-id="16774-119">useContactApis</span></span> | <span data-ttu-id="16774-120">`boolean` — Указывает, может ли компонент карточки контакта использовать API контактов Microsoft Graph для поиска контактных данных и фотографий.</span><span class="sxs-lookup"><span data-stu-id="16774-120">`boolean` - Indicates whether the person card component can use the Microsoft Graph Contact API to search for contact details and photos.</span></span> <span data-ttu-id="16774-121">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="16774-121">Default value is `true`.</span></span>  |
| <span data-ttu-id="16774-122">sections</span><span class="sxs-lookup"><span data-stu-id="16774-122">sections</span></span> | <span data-ttu-id="16774-123">`object` — Настройка отображения разделов в карточке контакта.</span><span class="sxs-lookup"><span data-stu-id="16774-123">`object` - Configures what sections are shown in the person card.</span></span>  |

### <a name="person-card-sections"></a><span data-ttu-id="16774-124">Разделы карточки контакта</span><span class="sxs-lookup"><span data-stu-id="16774-124">Person card sections</span></span>

<span data-ttu-id="16774-125">Карточка контакта содержит несколько настраиваемых разделов, в которых отображаются сведения о пользователе:</span><span class="sxs-lookup"><span data-stu-id="16774-125">The person card contains several configurable sections for displaying person details:</span></span>
* <span data-ttu-id="16774-126">Контакт — контактные данные, такие как электронная почта, номер телефона, должность, расположение и другие сведения.</span><span class="sxs-lookup"><span data-stu-id="16774-126">Contact - Contact information such as email, phone, position, location, and more.</span></span>
* <span data-ttu-id="16774-127">Организация — организационная диаграмма с руководителями, подчиненными или важными пользователями.</span><span class="sxs-lookup"><span data-stu-id="16774-127">Organization - Organizational graph with managers, direct reports, and relevant people.</span></span>
* <span data-ttu-id="16774-128">Сообщения — наиболее актуальные сообщения электронной почты вошедшего в систему пользователя.</span><span class="sxs-lookup"><span data-stu-id="16774-128">Messages - Most relevant email messages with the current signed in user.</span></span>
* <span data-ttu-id="16774-129">Файлы — наиболее актуальные общие файлы вошедшего в систему пользователя.</span><span class="sxs-lookup"><span data-stu-id="16774-129">Files - Most relevant shared files with the current signed in user.</span></span>
* <span data-ttu-id="16774-130">Профиль — информация о профиле, например проекты, навыки, языки и другие сведения.</span><span class="sxs-lookup"><span data-stu-id="16774-130">Profile - Profile information such as projects, skills, languages, and more.</span></span>

<span data-ttu-id="16774-131">Разделы загружаются по умолчанию, но их можно отключить глобально с помощью свойства объекта `MgtPersonCard.config.sections`.</span><span class="sxs-lookup"><span data-stu-id="16774-131">Sections are loaded by default, but they can be disabled globally via the `MgtPersonCard.config.sections` object property.</span></span> <span data-ttu-id="16774-132">Для редактирования доступны следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="16774-132">The following properties are available.</span></span>

| <span data-ttu-id="16774-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="16774-133">Property</span></span> | <span data-ttu-id="16774-134">Описание</span><span class="sxs-lookup"><span data-stu-id="16774-134">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="16774-135">organization;</span><span class="sxs-lookup"><span data-stu-id="16774-135">organization</span></span> | <span data-ttu-id="16774-136">`boolean` — указывает, отображается ли раздел организации карточки контакта.</span><span class="sxs-lookup"><span data-stu-id="16774-136">`boolean` - Indicates whether the person card organization section is shown.</span></span> <span data-ttu-id="16774-137">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="16774-137">Default value is `true`.</span></span>  |
| <span data-ttu-id="16774-138">mailMessages</span><span class="sxs-lookup"><span data-stu-id="16774-138">mailMessages</span></span> | <span data-ttu-id="16774-139">`boolean` — указывает, отображается ли раздел сообщений карточки контакта.</span><span class="sxs-lookup"><span data-stu-id="16774-139">`boolean` - Indicates whether the person card messages section is shown.</span></span> <span data-ttu-id="16774-140">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="16774-140">Default value is `true`.</span></span>  |
| <span data-ttu-id="16774-141">files</span><span class="sxs-lookup"><span data-stu-id="16774-141">files</span></span> | <span data-ttu-id="16774-142">`boolean` — указывает, отображается ли раздела файлов карточки контакта.</span><span class="sxs-lookup"><span data-stu-id="16774-142">`boolean` - Indicates whether the person card files section is shown.</span></span> <span data-ttu-id="16774-143">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="16774-143">Default value is `true`.</span></span>  |
| <span data-ttu-id="16774-144">profile</span><span class="sxs-lookup"><span data-stu-id="16774-144">profile</span></span> | <span data-ttu-id="16774-145">`boolean` — указывает, отображается ли раздел профиля карточки контакта.</span><span class="sxs-lookup"><span data-stu-id="16774-145">`boolean` - Indicates whether the person card profile section is shown.</span></span> <span data-ttu-id="16774-146">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="16774-146">Default value is `true`.</span></span>  |

<span data-ttu-id="16774-147">Чтобы отключить раздел, просто установите свойство в коде инициализации `false` приложения:</span><span class="sxs-lookup"><span data-stu-id="16774-147">To disable a section, simply set the property to `false` in your app initialization code:</span></span>
```ts
import { MgtPersonCard } from `@microsoft/mgt`;

MgtPersonCard.config.sections.profile = false;
```

## <a name="setup-for-teams-integrations"></a><span data-ttu-id="16774-148">Настройка интеграции с Teams</span><span class="sxs-lookup"><span data-stu-id="16774-148">Setup for Teams integrations</span></span>

<span data-ttu-id="16774-149">Компонент Person-Card позволяет связаться с целевым контактом, в том числе с помощью чата в Teams.</span><span class="sxs-lookup"><span data-stu-id="16774-149">The Person-Card component allows the user to contact the target person, including via Teams chat.</span></span> <span data-ttu-id="16774-150">При использовании компонента во вкладке приложения Teams можно сделать так, чтобы компонент не открывал окно браузера, а сразу переходил к чату, настроив `microsoftTeamsLib` в `TeamsProvider`.</span><span class="sxs-lookup"><span data-stu-id="16774-150">If using the component inside a Teams tab app, you can ensure that the component deep links directly to a chat instead of opening a browser window by setting the `microsoftTeamsLib` in `TeamsProvider`.</span></span>

<span data-ttu-id="16774-151">Если компоненту Person-Card не удается обнаружить библиотеку Teams, компонент пытается открыть веб-клиент Teams.</span><span class="sxs-lookup"><span data-stu-id="16774-151">If the Person-Card component is unable to detect the Teams lib, the component will attempt to open the Teams web client instead.</span></span>

```ts
import * as microsoftTeams from "@microsoft/teams-js";
import {TeamsHelper} from '@microsoft/mgt';

TeamsHelper.microsoftTeamsLib = microsoftTeams;
```

<span data-ttu-id="16774-152">Дополнительные сведения о поставщике `TeamsProvider` см. в статье ["Поставщик Microsoft Teams"](../providers/teams.md).</span><span class="sxs-lookup"><span data-stu-id="16774-152">For more information about the `TeamsProvider` provider, see [Microsoft Teams provider](../providers/teams.md).</span></span>

## <a name="properties"></a><span data-ttu-id="16774-153">Свойства</span><span class="sxs-lookup"><span data-stu-id="16774-153">Properties</span></span>

<span data-ttu-id="16774-154">По умолчанию компонент `mgt-person` передает сведения о пользователе `mgt-person-card` компоненту.</span><span class="sxs-lookup"><span data-stu-id="16774-154">By default, the `mgt-person` component will pass the person details to the `mgt-person-card` component.</span></span> <span data-ttu-id="16774-155">Однако эти атрибуты можно использовать для изменения такого поведения при создании шаблонов компонента `mgt-person` или при использовании компонента `mgt-person-card` в качестве отдельного компонента.</span><span class="sxs-lookup"><span data-stu-id="16774-155">However, you can use these attributes to change this when templating the `mgt-person` component or when using the `mgt-person-card` component as a standalone component.</span></span>

| <span data-ttu-id="16774-156">Атрибут</span><span class="sxs-lookup"><span data-stu-id="16774-156">Attribute</span></span>         | <span data-ttu-id="16774-157">Тип</span><span class="sxs-lookup"><span data-stu-id="16774-157">Type</span></span>                     | <span data-ttu-id="16774-158">Описание</span><span class="sxs-lookup"><span data-stu-id="16774-158">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="16774-159">person-details</span><span class="sxs-lookup"><span data-stu-id="16774-159">person-details</span></span> | <span data-ttu-id="16774-160">MicrosoftGraph.User</span><span class="sxs-lookup"><span data-stu-id="16774-160">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="16774-161">MicrosoftGraph.Person</span><span class="sxs-lookup"><span data-stu-id="16774-161">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="16774-162">MicrosoftGraph.Contact</span><span class="sxs-lookup"><span data-stu-id="16774-162">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="16774-163">Объект пользователя, определенный в Microsoft Graph и содержащий подробные сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="16774-163">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="16774-164">person-image</span><span class="sxs-lookup"><span data-stu-id="16774-164">person-image</span></span>   | <span data-ttu-id="16774-165">string</span><span class="sxs-lookup"><span data-stu-id="16774-165">string</span></span>                    | <span data-ttu-id="16774-166">Универсальный код ресурса (URI) изображения, связанный с человеком, который отображается в карточке.</span><span class="sxs-lookup"><span data-stu-id="16774-166">Image uri related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="16774-167">inherit-details</span><span class="sxs-lookup"><span data-stu-id="16774-167">inherit-details</span></span>   | <span data-ttu-id="16774-168">Отсутствует.</span><span class="sxs-lookup"><span data-stu-id="16774-168">None.</span></span>                  | <span data-ttu-id="16774-169">Разрешает проработку дерева родителей для компонента `mgt-person` для использования одинаковых данных `person-details` и `person-image`.</span><span class="sxs-lookup"><span data-stu-id="16774-169">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |
| <span data-ttu-id="16774-170">user-id</span><span class="sxs-lookup"><span data-stu-id="16774-170">user-id</span></span> | <span data-ttu-id="16774-171">string</span><span class="sxs-lookup"><span data-stu-id="16774-171">string</span></span> | <span data-ttu-id="16774-172">Позволяет разработчикам поставлять пользовательский id для получения данных, показанных на компоненте person-card</span><span class="sxs-lookup"><span data-stu-id="16774-172">Allows developers to supply user-id to retrieve data shown on person-card component</span></span> |
| <span data-ttu-id="16774-173">person-query</span><span class="sxs-lookup"><span data-stu-id="16774-173">person-query</span></span> | <span data-ttu-id="16774-174">string</span><span class="sxs-lookup"><span data-stu-id="16774-174">string</span></span> | <span data-ttu-id="16774-175">Позволяет разработчикам поставлять запрос пользователя для получения данных, показанных на компоненте person-card</span><span class="sxs-lookup"><span data-stu-id="16774-175">Allows developers to supply person-query to retrieve data shown on person-card component</span></span> |


## <a name="templates"></a><span data-ttu-id="16774-176">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="16774-176">Templates</span></span>

<span data-ttu-id="16774-177">В компоненте Person-Card используются [шаблоны](../customize-components/templates.md), позволяющие добавлять и заменять части компонента.</span><span class="sxs-lookup"><span data-stu-id="16774-177">The Person-Card component uses [templates](../customize-components/templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="16774-178">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="16774-178">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="16774-179">Тип данных</span><span class="sxs-lookup"><span data-stu-id="16774-179">Data type</span></span> | <span data-ttu-id="16774-180">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="16774-180">Data context</span></span> | <span data-ttu-id="16774-181">Описание</span><span class="sxs-lookup"><span data-stu-id="16774-181">Description</span></span> |
| - | - | - |
| <span data-ttu-id="16774-182">no-data</span><span class="sxs-lookup"><span data-stu-id="16774-182">no-data</span></span> | <span data-ttu-id="16774-183">null</span><span class="sxs-lookup"><span data-stu-id="16774-183">null</span></span> | <span data-ttu-id="16774-184">Шаблон, используемый, если данные недоступны.</span><span class="sxs-lookup"><span data-stu-id="16774-184">The template used when no data is available.</span></span>
| <span data-ttu-id="16774-185">default</span><span class="sxs-lookup"><span data-stu-id="16774-185">default</span></span> | <span data-ttu-id="16774-186">`person`: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="16774-186">`person`: The person details object</span></span> <br> <span data-ttu-id="16774-187">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="16774-187">`personImage`: The URL of the image</span></span> | <span data-ttu-id="16774-188">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="16774-188">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="16774-189">person-details</span><span class="sxs-lookup"><span data-stu-id="16774-189">person-details</span></span> | <span data-ttu-id="16774-190">`person`: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="16774-190">`person`: The person details object</span></span> | <span data-ttu-id="16774-191">Шаблон, используемый для отображения верхней части карточки пользователя.</span><span class="sxs-lookup"><span data-stu-id="16774-191">The template used to render the top part of the person card.</span></span> |
| <span data-ttu-id="16774-192">additional-details</span><span class="sxs-lookup"><span data-stu-id="16774-192">additional-details</span></span> | <span data-ttu-id="16774-193">`person`: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="16774-193">`person`: The person details object</span></span> <br> <span data-ttu-id="16774-194">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="16774-194">`personImage`: the URL of the image</span></span> | <span data-ttu-id="16774-195">Шаблон, который используется для добавления настраиваемого контента в контейнер дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="16774-195">The template used to add custom content to the additional details container.</span></span> |

<span data-ttu-id="16774-196">Например, шаблон можно использовать для настройки компонента, вложенного в компонент `mgt-person`, и шаблона, чтобы добавить дополнительные сведения в карточку.</span><span class="sxs-lookup"><span data-stu-id="16774-196">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="events"></a><span data-ttu-id="16774-197">События</span><span class="sxs-lookup"><span data-stu-id="16774-197">Events</span></span>

<span data-ttu-id="16774-198">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="16774-198">The following events are fired from the component.</span></span>

| <span data-ttu-id="16774-199">Событие</span><span class="sxs-lookup"><span data-stu-id="16774-199">Event</span></span> | <span data-ttu-id="16774-200">Описание</span><span class="sxs-lookup"><span data-stu-id="16774-200">Description</span></span> |
| --- | --- |
| `expanded` | <span data-ttu-id="16774-201">Пользователь открыл расширенный раздел сведений карты.</span><span class="sxs-lookup"><span data-stu-id="16774-201">The user has opened the expanded details section of the card.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="16774-202">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="16774-202">CSS custom properties</span></span>

<span data-ttu-id="16774-203">Компонент `mgt-person-card` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="16774-203">The `mgt-person-card` component defines the following CSS custom properties.</span></span> 

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

<span data-ttu-id="16774-204">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="16774-204">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="16774-205">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="16774-205">Microsoft Graph permissions</span></span>

<span data-ttu-id="16774-206">Этот элемент управления Person-Card использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="16774-206">The Person-Card control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="16774-207">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="16774-207">Configuration</span></span> | <span data-ttu-id="16774-208">Разрешение</span><span class="sxs-lookup"><span data-stu-id="16774-208">Permission</span></span> | <span data-ttu-id="16774-209">API</span><span class="sxs-lookup"><span data-stu-id="16774-209">API</span></span> | <span data-ttu-id="16774-210">Section</span><span class="sxs-lookup"><span data-stu-id="16774-210">Section</span></span> |
| --- | ---------- | ------- | --------- |
| <span data-ttu-id="16774-211">`personDetails` установить с `id` пользователем, но без электронной почты, или `userId` установить, или `personQuery` установить `me`</span><span class="sxs-lookup"><span data-stu-id="16774-211">`personDetails` set with user's `id` but without e-mail, or `userId` set, or `personQuery` set to `me`</span></span> | <span data-ttu-id="16774-212">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="16774-212">User.ReadBasic.All</span></span> | <span data-ttu-id="16774-213">[/users/{id}](/graph/api/user-list-people), [/users/{id}/photo/$value](/graph/api/profilephoto-get)</span><span class="sxs-lookup"><span data-stu-id="16774-213">[/users/{id}](/graph/api/user-list-people), [/users/{id}/photo/$value](/graph/api/profilephoto-get)</span></span> | <span data-ttu-id="16774-214">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="16774-214">Default</span></span> |
| <span data-ttu-id="16774-215">`personQuery` значение, отличаее от `me`</span><span class="sxs-lookup"><span data-stu-id="16774-215">`personQuery` set to a value different than `me`</span></span> | <span data-ttu-id="16774-216">People.Read</span><span class="sxs-lookup"><span data-stu-id="16774-216">People.Read</span></span> | [<span data-ttu-id="16774-217">/me/people/?$search=</span><span class="sxs-lookup"><span data-stu-id="16774-217">/me/people/?$search=</span></span>](/graph/api/user-list-people) | <span data-ttu-id="16774-218">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="16774-218">Default</span></span> |
| <span data-ttu-id="16774-219">`personQuery` установлено значение, отличаее от значения `me` `config.useContactApis` `true` (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="16774-219">`personQuery` set to a value different than `me` and `config.useContactApis` set to `true` (default)</span></span> | <span data-ttu-id="16774-220">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="16774-220">Contacts.Read</span></span> | [<span data-ttu-id="16774-221">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="16774-221">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="16774-222">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="16774-222">Default</span></span> |
| <span data-ttu-id="16774-223">`showPresence` установлено, что `true`</span><span class="sxs-lookup"><span data-stu-id="16774-223">`showPresence` set to `true`</span></span> | <span data-ttu-id="16774-224">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="16774-224">Presence.Read.All</span></span> | [<span data-ttu-id="16774-225">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="16774-225">/users/{id}/presence</span></span>](/graph/api/presence-get) | <span data-ttu-id="16774-226">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="16774-226">Default</span></span> |
| <span data-ttu-id="16774-227">`sections.organization` включено (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="16774-227">`sections.organization` enabled (default)</span></span> | <span data-ttu-id="16774-228">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="16774-228">User.Read.All</span></span> | [<span data-ttu-id="16774-229">/users/{id}/manager</span><span class="sxs-lookup"><span data-stu-id="16774-229">/users/{id}/manager</span></span>](/graph/api/user-list-manager) | <span data-ttu-id="16774-230">Организация</span><span class="sxs-lookup"><span data-stu-id="16774-230">Organization</span></span> |
| <span data-ttu-id="16774-231">`sections.organization.showWorksWith` set (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="16774-231">`sections.organization.showWorksWith` set (default)</span></span> | <span data-ttu-id="16774-232">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="16774-232">People.Read.All</span></span> | [<span data-ttu-id="16774-233">/users/{id}/people</span><span class="sxs-lookup"><span data-stu-id="16774-233">/users/{id}/people</span></span>](/graph/api/user-list-people) | <span data-ttu-id="16774-234">Организация</span><span class="sxs-lookup"><span data-stu-id="16774-234">Organization</span></span> |
| <span data-ttu-id="16774-235">`sections.mailMessages` включено (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="16774-235">`sections.mailMessages` enabled (default)</span></span> | <span data-ttu-id="16774-236">Mail.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="16774-236">Mail.ReadBasic</span></span> | [<span data-ttu-id="16774-237">/me/messages</span><span class="sxs-lookup"><span data-stu-id="16774-237">/me/messages</span></span>](/graph/api/user-list-messages) | <span data-ttu-id="16774-238">Сообщения</span><span class="sxs-lookup"><span data-stu-id="16774-238">Messages</span></span> |
| <span data-ttu-id="16774-239">`sections.files` включено (по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="16774-239">`sections.files` enabled (default)</span></span> | <span data-ttu-id="16774-240">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="16774-240">Sites.Read.All</span></span> | <span data-ttu-id="16774-241">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span><span class="sxs-lookup"><span data-stu-id="16774-241">[/me/insights/shared](/graph/api/insights-list-shared) and [/me/insights/used](/graph/api/insights-list-used)</span></span> | <span data-ttu-id="16774-242">Файлы</span><span class="sxs-lookup"><span data-stu-id="16774-242">Files</span></span> |

<span data-ttu-id="16774-243">Класс `MgtPersonCard` также предоставляет `getScopes` статический метод, возвращающий массив областей, необходимый для работы карточки контакта с учетом глобальной конфигурации карточки контакта.</span><span class="sxs-lookup"><span data-stu-id="16774-243">The `MgtPersonCard` class also exposes a `getScopes` static method that returns an array of scopes required for the person card to function based on the global person card configuration.</span></span>

```ts
import { MgtPersonCard } from `@microsoft/mgt`;

const neededScopes = MgtPersonCard.getScopes();
```

## <a name="authentication"></a><span data-ttu-id="16774-244">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="16774-244">Authentication</span></span>

<span data-ttu-id="16774-245">В элементе управления Person-Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="16774-245">The Person-Card control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span> 

## <a name="cache"></a><span data-ttu-id="16774-246">Кэш</span><span class="sxs-lookup"><span data-stu-id="16774-246">Cache</span></span>

> [!IMPORTANT]
> <span data-ttu-id="16774-247">Компонент `mgt-person-card` извлекает основные данные человека из родительского компонента, `mgt-person` не вызывая Graph.</span><span class="sxs-lookup"><span data-stu-id="16774-247">The `mgt-person-card` component retrieves the basic person data from the parent `mgt-person` component without calling Microsoft Graph.</span></span> <span data-ttu-id="16774-248">Когда используется отдельно, он извлекает необходимые данные и `mgt-person-card` кэширует их.</span><span class="sxs-lookup"><span data-stu-id="16774-248">When `mgt-person-card` is used separately, it will retrieve the necessary data itself and cache it.</span></span> <span data-ttu-id="16774-249">Данные, отображаемые в разделах карты, извлекаются отдельно и не кэшются.</span><span class="sxs-lookup"><span data-stu-id="16774-249">The data displayed in card's sections is retrieved separately and is not cached.</span></span>

|<span data-ttu-id="16774-250">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="16774-250">Object store</span></span>|<span data-ttu-id="16774-251">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="16774-251">Cached data</span></span>|<span data-ttu-id="16774-252">Примечания</span><span class="sxs-lookup"><span data-stu-id="16774-252">Remarks</span></span>|
|---------|-----------|-------|
|`people`|<span data-ttu-id="16774-253">Сведения о человеке</span><span class="sxs-lookup"><span data-stu-id="16774-253">Person's information</span></span>|<span data-ttu-id="16774-254">Используется при `personQuery` указании и его значение отличается от `me`</span><span class="sxs-lookup"><span data-stu-id="16774-254">Used when `personQuery` is specified and its value is different than `me`</span></span>|
|`photos`|<span data-ttu-id="16774-255">Фотография человека</span><span class="sxs-lookup"><span data-stu-id="16774-255">Person's photo</span></span>|
|`presence`|<span data-ttu-id="16774-256">Присутствие человека</span><span class="sxs-lookup"><span data-stu-id="16774-256">Person's presence</span></span>|<span data-ttu-id="16774-257">Используется, `showPresence` когда установлено `true`</span><span class="sxs-lookup"><span data-stu-id="16774-257">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="16774-258">Сведения о пользователях</span><span class="sxs-lookup"><span data-stu-id="16774-258">Person's user information</span></span>|<span data-ttu-id="16774-259">Используется при `userId` указании или `personQuery` задан `me`</span><span class="sxs-lookup"><span data-stu-id="16774-259">Used when `userId` is specified or the `personQuery` is set to `me`</span></span>|

<span data-ttu-id="16774-260">Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="16774-260">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>
