---
title: Компонент пользователя в Microsoft Graph Toolkit
description: Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, имени и/или адреса электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 3020c652fa08c78fecd53469af0e21622f9afcff
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780997"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="992b9-103">Компонент пользователя в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="992b9-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="992b9-104">Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, адреса электронной почты и любых других сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="992b9-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="992b9-105">Кроме того, в компоненте пользователя используется [mgt-person-card](./person-card.md) для отображения карточки всплывающего окна с дополнительной информации о пользователе.</span><span class="sxs-lookup"><span data-stu-id="992b9-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="992b9-106">Дополнительные сведения см. в разделе [Карточка пользователя](#person-card).</span><span class="sxs-lookup"><span data-stu-id="992b9-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="992b9-107">Пример</span><span class="sxs-lookup"><span data-stu-id="992b9-107">Example</span></span>

<span data-ttu-id="992b9-108">В приведенном далее примере показан пользователь, использующий компонент `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="992b9-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="992b9-109">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="992b9-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="992b9-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="992b9-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="992b9-111">Настройка сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="992b9-111">Setting the person details</span></span>

<span data-ttu-id="992b9-112">Чтобы задать сведения о пользователе, можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="992b9-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="992b9-113">Используйте только одно из указанных далее свойств для одного случая:</span><span class="sxs-lookup"><span data-stu-id="992b9-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="992b9-114">Задайте атрибут `user-id` или свойство `userId`, чтобы получить данные пользователя из Microsoft Graph, используя его идентификатор.</span><span class="sxs-lookup"><span data-stu-id="992b9-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="992b9-115">Чтобы выполнить поиск определенного пользователя в Microsoft Graph, задайте атрибут `person-query` или свойство `personQuery`.</span><span class="sxs-lookup"><span data-stu-id="992b9-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="992b9-116">При этом будет выбран первый доступный пользователь и будут получены сведения об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="992b9-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="992b9-117">Электронная почта лучше всего подходит для того, чтобы найти нужного пользователя, но можно использовать и имя.</span><span class="sxs-lookup"><span data-stu-id="992b9-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="992b9-118">Задайте атрибут `person-presence` или свойство `personPresence`, чтобы добавить значок присутствия в аватар пользователя вручную.</span><span class="sxs-lookup"><span data-stu-id="992b9-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="992b9-119">Чтобы определить размер аватара, задайте для атрибута `avatar-size` или свойства `avatarSize` значение `small` или `large`.</span><span class="sxs-lookup"><span data-stu-id="992b9-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="992b9-120">Это позволяет добавить [правильный значок присутствия](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) в аватар.</span><span class="sxs-lookup"><span data-stu-id="992b9-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="992b9-121">Чтобы дополнительно настроить размер аватара, вам нужно выбрать соответствующие настраиваемые свойства CSS, указанные далее.</span><span class="sxs-lookup"><span data-stu-id="992b9-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="992b9-122">Для этого параметра по умолчанию задано значение `auto`, благодаря которому присутствие будет обрабатываться автоматически с учетом свойства `view`.</span><span class="sxs-lookup"><span data-stu-id="992b9-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="992b9-123">Рекомендуем использовать `small`, если аватар меньше 32 на 32 пикс.</span><span class="sxs-lookup"><span data-stu-id="992b9-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="992b9-124">Чтобы вручную задать сведения о пользователе, используйте атрибут `person-details` или свойство `personDetails`, как показано в приведенном далее примере.</span><span class="sxs-lookup"><span data-stu-id="992b9-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="992b9-125">Если изображение не предоставлено, оно будет получено (при наличии).</span><span class="sxs-lookup"><span data-stu-id="992b9-125">If no image is provided, one will be fetched (if available).</span></span>

* <span data-ttu-id="992b9-126">По умолчанию компонент пользователя запрашивает только стандартный набор свойств Graph [Майкрософт.](/graph/api/user-get?&tabs=http#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="992b9-126">By default, the person component will only request the standard Microsoft Graph user set of [properties](/graph/api/user-get?&tabs=http#optional-query-parameters).</span></span> <span data-ttu-id="992b9-127">Чтобы запросить дополнительные свойства, объявите их в качестве любой части `line(x)Property` .</span><span class="sxs-lookup"><span data-stu-id="992b9-127">In order to request additional properties, declare them as any part of the `line(x)Property`.</span></span> 


## <a name="properties"></a><span data-ttu-id="992b9-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="992b9-128">Properties</span></span>

<span data-ttu-id="992b9-129">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="992b9-129">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="992b9-130">Атрибут</span><span class="sxs-lookup"><span data-stu-id="992b9-130">Attribute</span></span>       | <span data-ttu-id="992b9-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="992b9-131">Property</span></span>       | <span data-ttu-id="992b9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="992b9-132">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="992b9-133">user-id</span><span class="sxs-lookup"><span data-stu-id="992b9-133">user-id</span></span>         | <span data-ttu-id="992b9-134">userId</span><span class="sxs-lookup"><span data-stu-id="992b9-134">userId</span></span>         | <span data-ttu-id="992b9-135">Установите идентификатор пользователя, чтобы получить сведения об этом пользователе и его изображение из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="992b9-135">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="992b9-136">person-query</span><span class="sxs-lookup"><span data-stu-id="992b9-136">person-query</span></span>    | <span data-ttu-id="992b9-137">personQuery</span><span class="sxs-lookup"><span data-stu-id="992b9-137">personQuery</span></span>    | <span data-ttu-id="992b9-138">Чтобы найти пользователя в Microsoft Graph, установите его имя или адрес электронной почты пользователя и получите сведения о первом пользователе и его изображение.</span><span class="sxs-lookup"><span data-stu-id="992b9-138">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="992b9-139">person-details</span><span class="sxs-lookup"><span data-stu-id="992b9-139">person-details</span></span>  | <span data-ttu-id="992b9-140">personDetails</span><span class="sxs-lookup"><span data-stu-id="992b9-140">personDetails</span></span>  | <span data-ttu-id="992b9-141">Установите объект, представляющий пользователя.</span><span class="sxs-lookup"><span data-stu-id="992b9-141">Set to an object representing a person.</span></span> <span data-ttu-id="992b9-142">Используется для объекта из ресурсов "люди", "пользователи", "контакты" или "группа".</span><span class="sxs-lookup"><span data-stu-id="992b9-142">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="992b9-143">fallback-details</span><span class="sxs-lookup"><span data-stu-id="992b9-143">fallback-details</span></span>| <span data-ttu-id="992b9-144">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="992b9-144">fallbackDetails</span></span>| <span data-ttu-id="992b9-145">Установите объект, представляющий человека, если в графе не обнаружено пользователя/пользователя/контакта.</span><span class="sxs-lookup"><span data-stu-id="992b9-145">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="992b9-146">person-image</span><span class="sxs-lookup"><span data-stu-id="992b9-146">person-image</span></span>    | <span data-ttu-id="992b9-147">personImage</span><span class="sxs-lookup"><span data-stu-id="992b9-147">personImage</span></span>    | <span data-ttu-id="992b9-148">Задать изображение, которое будет отображаться для пользователя.</span><span class="sxs-lookup"><span data-stu-id="992b9-148">Set the image to show for the person.</span></span> |
| <span data-ttu-id="992b9-149">person-presence</span><span class="sxs-lookup"><span data-stu-id="992b9-149">person-presence</span></span> | <span data-ttu-id="992b9-150">personPresence</span><span class="sxs-lookup"><span data-stu-id="992b9-150">personPresence</span></span> | <span data-ttu-id="992b9-151">Установка присутствия для пользователя.</span><span class="sxs-lookup"><span data-stu-id="992b9-151">Set the presence for the person.</span></span> |
| <span data-ttu-id="992b9-152">fetch-image</span><span class="sxs-lookup"><span data-stu-id="992b9-152">fetch-image</span></span>     | <span data-ttu-id="992b9-153">fetchImage</span><span class="sxs-lookup"><span data-stu-id="992b9-153">fetchImage</span></span>     | <span data-ttu-id="992b9-154">Установите флажок для автоматического получения `personImage` из Microsoft Graph на основе объекта `personDetails`, предоставленного пользователем.</span><span class="sxs-lookup"><span data-stu-id="992b9-154">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="992b9-155">тип аватара</span><span class="sxs-lookup"><span data-stu-id="992b9-155">avatar-type</span></span>     | <span data-ttu-id="992b9-156">avatarType</span><span class="sxs-lookup"><span data-stu-id="992b9-156">avatarType</span></span>     | <span data-ttu-id="992b9-157">Установите или `initials` `photo` отобразить состояние отображения по умолчанию — это фотография.</span><span class="sxs-lookup"><span data-stu-id="992b9-157">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="992b9-158">представление</span><span class="sxs-lookup"><span data-stu-id="992b9-158">view</span></span>            | <span data-ttu-id="992b9-159">представление</span><span class="sxs-lookup"><span data-stu-id="992b9-159">view</span></span>           | <span data-ttu-id="992b9-160">Установите, чтобы настроить, как выглядит пользователь.</span><span class="sxs-lookup"><span data-stu-id="992b9-160">Set to control how the person is rendered.</span></span> <span data-ttu-id="992b9-161">Значение по умолчанию: `avatar`</span><span class="sxs-lookup"><span data-stu-id="992b9-161">Default is `avatar`</span></span> <br /> <span data-ttu-id="992b9-162">`avatar` — Показывать только аватар</span><span class="sxs-lookup"><span data-stu-id="992b9-162">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="992b9-163">`oneline` — Показывать аватар и первую строку (`displayName` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="992b9-163">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="992b9-164">`twolines` — Показывать аватар и две строки текста (`displayName` и `mail` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="992b9-164">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="992b9-165">line1-property</span><span class="sxs-lookup"><span data-stu-id="992b9-165">line1-property</span></span>  | <span data-ttu-id="992b9-166">line1Property</span><span class="sxs-lookup"><span data-stu-id="992b9-166">line1Property</span></span>  | <span data-ttu-id="992b9-167">Задает свойство personDetails для использования для первой строки текста.</span><span class="sxs-lookup"><span data-stu-id="992b9-167">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="992b9-168">Значение по умолчанию: `displayName`.</span><span class="sxs-lookup"><span data-stu-id="992b9-168">Default is `displayName`.</span></span>|
| <span data-ttu-id="992b9-169">line2-property</span><span class="sxs-lookup"><span data-stu-id="992b9-169">line2-property</span></span>  | <span data-ttu-id="992b9-170">line2Property</span><span class="sxs-lookup"><span data-stu-id="992b9-170">line2Property</span></span>  | <span data-ttu-id="992b9-171">Задает свойство personDetails для использования для второй строки текста.</span><span class="sxs-lookup"><span data-stu-id="992b9-171">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="992b9-172">Значение по умолчанию: `mail`.</span><span class="sxs-lookup"><span data-stu-id="992b9-172">Default is `mail`.</span></span>|
| <span data-ttu-id="992b9-173">line3-property</span><span class="sxs-lookup"><span data-stu-id="992b9-173">line3-property</span></span>  | <span data-ttu-id="992b9-174">line3Property</span><span class="sxs-lookup"><span data-stu-id="992b9-174">line3Property</span></span>  | <span data-ttu-id="992b9-175">Задает свойство personDetails для использования для третьей строки текста.</span><span class="sxs-lookup"><span data-stu-id="992b9-175">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="992b9-176">Значение по умолчанию: `jobTitle`.</span><span class="sxs-lookup"><span data-stu-id="992b9-176">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="992b9-177">show-presence</span><span class="sxs-lookup"><span data-stu-id="992b9-177">show-presence</span></span>   | <span data-ttu-id="992b9-178">showPresence</span><span class="sxs-lookup"><span data-stu-id="992b9-178">showPresence</span></span>   | <span data-ttu-id="992b9-179">Установить флажок отображения присутствия пользователя — по умолчанию `false`.</span><span class="sxs-lookup"><span data-stu-id="992b9-179">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="992b9-180">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="992b9-180">CSS custom properties</span></span>

<span data-ttu-id="992b9-181">Компонент `mgt-person` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="992b9-181">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --avatar-cursor: default;
  
  --initials-color: white;
  --initials-background-color: magenta;

  --presence-background-color: #ffffff;
  --presence-icon-color: #ffffff;

  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --text-transform: none;

  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;

  --line3-font-size: 12px;
  --line3-font-weight: 400;
  --line3-color: black;
  --line3-text-transform: none;

  --details-spacing: 12px;
}
```

<span data-ttu-id="992b9-182">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="992b9-182">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="992b9-183">События</span><span class="sxs-lookup"><span data-stu-id="992b9-183">Events</span></span>

<span data-ttu-id="992b9-184">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="992b9-184">The following events are fired from the component.</span></span>

| <span data-ttu-id="992b9-185">Событие</span><span class="sxs-lookup"><span data-stu-id="992b9-185">Event</span></span> | <span data-ttu-id="992b9-186">Сведения</span><span class="sxs-lookup"><span data-stu-id="992b9-186">Detail</span></span> | <span data-ttu-id="992b9-187">Описание</span><span class="sxs-lookup"><span data-stu-id="992b9-187">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="992b9-188">line1clicked</span><span class="sxs-lookup"><span data-stu-id="992b9-188">line1clicked</span></span> | <span data-ttu-id="992b9-189">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="992b9-189">The detail contains the respective `person` object</span></span> | <span data-ttu-id="992b9-190">Уволено при нажатии строки 1.</span><span class="sxs-lookup"><span data-stu-id="992b9-190">Fired when line1 is clicked.</span></span> |
| <span data-ttu-id="992b9-191">line2clicked</span><span class="sxs-lookup"><span data-stu-id="992b9-191">line2clicked</span></span> | <span data-ttu-id="992b9-192">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="992b9-192">The detail contains the respective `person` object</span></span> | <span data-ttu-id="992b9-193">Уволено при нажатии строки2.</span><span class="sxs-lookup"><span data-stu-id="992b9-193">Fired when line2 is clicked.</span></span> |
| <span data-ttu-id="992b9-194">line3clicked</span><span class="sxs-lookup"><span data-stu-id="992b9-194">line3clicked</span></span> | <span data-ttu-id="992b9-195">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="992b9-195">The detail contains the respective `person` object</span></span> | <span data-ttu-id="992b9-196">Уволено при нажатии строки 3.</span><span class="sxs-lookup"><span data-stu-id="992b9-196">Fired when line3 is clicked.</span></span> |

## <a name="templates"></a><span data-ttu-id="992b9-197">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="992b9-197">Templates</span></span>

<span data-ttu-id="992b9-198">Компонент `mgt-person` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="992b9-198">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="992b9-199">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="992b9-199">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="992b9-200">Тип данных</span><span class="sxs-lookup"><span data-stu-id="992b9-200">Data type</span></span> | <span data-ttu-id="992b9-201">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="992b9-201">Data context</span></span> | <span data-ttu-id="992b9-202">Описание</span><span class="sxs-lookup"><span data-stu-id="992b9-202">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="992b9-203">загрузка</span><span class="sxs-lookup"><span data-stu-id="992b9-203">loading</span></span> | <span data-ttu-id="992b9-204">Нет</span><span class="sxs-lookup"><span data-stu-id="992b9-204">none</span></span> | <span data-ttu-id="992b9-205">Шаблон для отображения состояния загрузки компонента.</span><span class="sxs-lookup"><span data-stu-id="992b9-205">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="992b9-206">no-data</span><span class="sxs-lookup"><span data-stu-id="992b9-206">no-data</span></span> | <span data-ttu-id="992b9-207">Нет</span><span class="sxs-lookup"><span data-stu-id="992b9-207">none</span></span> | <span data-ttu-id="992b9-208">Шаблон для использования, если изображения или данные не доступны.</span><span class="sxs-lookup"><span data-stu-id="992b9-208">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="992b9-209">default</span><span class="sxs-lookup"><span data-stu-id="992b9-209">default</span></span> | <span data-ttu-id="992b9-210">пользователь: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="992b9-210">person: The person details object</span></span> <br> <span data-ttu-id="992b9-211">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="992b9-211">`personImage`: The URL of the image</span></span> <br> <span data-ttu-id="992b9-212">`personPresence`: Объект сведений о присутствии для человека</span><span class="sxs-lookup"><span data-stu-id="992b9-212">`personPresence`: The presence details object for person</span></span>  | <span data-ttu-id="992b9-213">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="992b9-213">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="992b9-214">person-card</span><span class="sxs-lookup"><span data-stu-id="992b9-214">person-card</span></span> | <span data-ttu-id="992b9-215">пользователь: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="992b9-215">person: The person details object</span></span> <br> <span data-ttu-id="992b9-216">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="992b9-216">`personImage`: The URL of the image</span></span> | <span data-ttu-id="992b9-217">Шаблон для обновления карточки mgt-person-card, отображаемой при наведении указателя мыши или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="992b9-217">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="992b9-218">line1</span><span class="sxs-lookup"><span data-stu-id="992b9-218">line1</span></span> | <span data-ttu-id="992b9-219">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="992b9-219">person: The person details object</span></span> | <span data-ttu-id="992b9-220">Шаблон для первой строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="992b9-220">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="992b9-221">line2</span><span class="sxs-lookup"><span data-stu-id="992b9-221">line2</span></span> | <span data-ttu-id="992b9-222">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="992b9-222">person: The person details object</span></span> | <span data-ttu-id="992b9-223">Шаблон для второй строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="992b9-223">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="992b9-224">line3</span><span class="sxs-lookup"><span data-stu-id="992b9-224">line3</span></span> | <span data-ttu-id="992b9-225">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="992b9-225">person: The person details object</span></span> | <span data-ttu-id="992b9-226">Шаблон для третьей строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="992b9-226">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="992b9-227">В следующем примере определяется шаблон для компонента пользователя.</span><span class="sxs-lookup"><span data-stu-id="992b9-227">The following example defines a template for the person component.</span></span>

```html
<!-- Retemplate the entire person component -->
<mgt-person>
  <template>
    <div data-if="personImage">
      <img src="{{personImage}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>

<!-- Retemplate the line properties -->
<mgt-person view="threeLines">
  <template data-type="line1">
    <div>
      Hello, my name is: {{person.displayName}}
    </div>
  </template>
  <template data-type="line2">
    <div>
      Super cool
    </div>
  </template>
  <template data-type="line3">
    <div>
      Loves MGT
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a><span data-ttu-id="992b9-228">Карточка пользователя</span><span class="sxs-lookup"><span data-stu-id="992b9-228">Person card</span></span>

<span data-ttu-id="992b9-229">`mgt-person` Компонент может отображаться`mgt-person-card` при либо наведении указателя мыши, либо щелчка мышью.</span><span class="sxs-lookup"><span data-stu-id="992b9-229">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="992b9-230">Добавьте средство управления на HTML-страницу.</span><span class="sxs-lookup"><span data-stu-id="992b9-230">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="992b9-231">Атрибут</span><span class="sxs-lookup"><span data-stu-id="992b9-231">Attribute</span></span>    |  <span data-ttu-id="992b9-232">Свойство</span><span class="sxs-lookup"><span data-stu-id="992b9-232">Property</span></span>     | <span data-ttu-id="992b9-233">Описание</span><span class="sxs-lookup"><span data-stu-id="992b9-233">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="992b9-234">person-card</span><span class="sxs-lookup"><span data-stu-id="992b9-234">person-card</span></span> | <span data-ttu-id="992b9-235">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="992b9-235">personCardInteraction</span></span> | <span data-ttu-id="992b9-236">Перечисление для определения пользовательского действия, необходимого для активации всплывающей панели — `hover` или `click`.</span><span class="sxs-lookup"><span data-stu-id="992b9-236">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="992b9-237">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="992b9-237">Default value is `none`</span></span> |


<span data-ttu-id="992b9-238">Дополнительные сведения о шаблонах, стилях и атрибутах см. в статье [Компонент карточки пользователя](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="992b9-238">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="992b9-239">Конфигурация глобального компонента</span><span class="sxs-lookup"><span data-stu-id="992b9-239">Global component configuration</span></span>

<span data-ttu-id="992b9-240">Класс `MgtPerson` предоставляет статический объект `config`, который конфигурирует все компоненты пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="992b9-240">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="992b9-241">В приведенном ниже примере показано, как использовать объект конфигурации.</span><span class="sxs-lookup"><span data-stu-id="992b9-241">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="992b9-242">Ниже указаны свойства, доступные в объекте конфигурации.</span><span class="sxs-lookup"><span data-stu-id="992b9-242">The following properties are available on the config object.</span></span>

| <span data-ttu-id="992b9-243">Свойство</span><span class="sxs-lookup"><span data-stu-id="992b9-243">Property</span></span> | <span data-ttu-id="992b9-244">Описание</span><span class="sxs-lookup"><span data-stu-id="992b9-244">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="992b9-245">useContactApis</span><span class="sxs-lookup"><span data-stu-id="992b9-245">useContactApis</span></span> | <span data-ttu-id="992b9-246">`boolean` — Указывает, может ли компонент пользователя использовать API личных контактов Microsoft Graph для поиска контактных данных и фотографий.</span><span class="sxs-lookup"><span data-stu-id="992b9-246">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="992b9-247">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="992b9-247">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="992b9-248">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="992b9-248">Microsoft Graph permissions</span></span>

<span data-ttu-id="992b9-249">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="992b9-249">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="992b9-250">Конфигурация</span><span class="sxs-lookup"><span data-stu-id="992b9-250">Configuration</span></span> | <span data-ttu-id="992b9-251">Разрешение</span><span class="sxs-lookup"><span data-stu-id="992b9-251">Permission</span></span> | <span data-ttu-id="992b9-252">API</span><span class="sxs-lookup"><span data-stu-id="992b9-252">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="992b9-253">`personDetails` установить без изображения, `fetchImage` установить , установить , `true` извлекаемого `avatarType` человека является контакт и `photo` `useContactApis` установить `true`</span><span class="sxs-lookup"><span data-stu-id="992b9-253">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo`, retrieved person is a contact and `useContactApis` set to `true`</span></span> | <span data-ttu-id="992b9-254">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="992b9-254">Contacts.Read</span></span> | [<span data-ttu-id="992b9-255">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="992b9-255">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) |
| <span data-ttu-id="992b9-256">`personDetails` установить без изображения, установить , установить и лицо не является `fetchImage` `true` `avatarType` `photo` контактом или `useContactApis` установлено, чтобы `false`</span><span class="sxs-lookup"><span data-stu-id="992b9-256">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and person is not a contact or `useContactApis` is set to `false`</span></span> | <span data-ttu-id="992b9-257">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="992b9-257">User.ReadBasic.All</span></span> | [<span data-ttu-id="992b9-258">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="992b9-258">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="992b9-259">`personDetails` набор без изображения, `fetchImage` установленный `true` для , `avatarType` заданный пользователем и `photo` указанный по электронной почте</span><span class="sxs-lookup"><span data-stu-id="992b9-259">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and user specified via email</span></span> | <span data-ttu-id="992b9-260">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="992b9-260">User.ReadBasic.All</span></span> | [<span data-ttu-id="992b9-261">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="992b9-261">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="992b9-262">`personDetails` набор без изображения, `fetchImage` `true` `avatarType` заданный, заданный и `photo` контакт, указанный по электронной почте</span><span class="sxs-lookup"><span data-stu-id="992b9-262">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and contact specified via email</span></span> | <span data-ttu-id="992b9-263">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="992b9-263">Contacts.Read</span></span> | [<span data-ttu-id="992b9-264">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="992b9-264">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) |
| <span data-ttu-id="992b9-265">`userId` set</span><span class="sxs-lookup"><span data-stu-id="992b9-265">`userId` set</span></span> | <span data-ttu-id="992b9-266">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="992b9-266">User.ReadBasic.All</span></span> | [<span data-ttu-id="992b9-267">/users/{id}</span><span class="sxs-lookup"><span data-stu-id="992b9-267">/users/{id}</span></span>](/graph/api/user-list-people) |
| <span data-ttu-id="992b9-268">`personQuery` установлено `me` и `avatarType` установлено `photo`</span><span class="sxs-lookup"><span data-stu-id="992b9-268">`personQuery` set to `me` and `avatarType` set to `photo`</span></span> | <span data-ttu-id="992b9-269">User.Read</span><span class="sxs-lookup"><span data-stu-id="992b9-269">User.Read</span></span> | [<span data-ttu-id="992b9-270">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="992b9-270">/me/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="992b9-271">`personQuery` установлено `me` и `avatarType` установлено что-то другое, чем `photo`</span><span class="sxs-lookup"><span data-stu-id="992b9-271">`personQuery` set to `me` and `avatarType` set to something else than `photo`</span></span> | <span data-ttu-id="992b9-272">User.Read</span><span class="sxs-lookup"><span data-stu-id="992b9-272">User.Read</span></span> | [<span data-ttu-id="992b9-273">/me</span><span class="sxs-lookup"><span data-stu-id="992b9-273">/me</span></span>](/graph/api/user-get) |
| <span data-ttu-id="992b9-274">`personQuery`значение, `me` заме- `useContactApis``true`</span><span class="sxs-lookup"><span data-stu-id="992b9-274">`personQuery` set to a value other than `me` and `useContactApis` set to `true`</span></span> | <span data-ttu-id="992b9-275">People.Read, User.ReadBasic.All, Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="992b9-275">People.Read, User.ReadBasic.All, Contacts.Read</span></span> | <span data-ttu-id="992b9-276">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/ \* ](/graph/api/user-list-contacts)</span><span class="sxs-lookup"><span data-stu-id="992b9-276">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/\*](/graph/api/user-list-contacts)</span></span> |
| <span data-ttu-id="992b9-277">`personQuery`значение, `me` заме- `useContactApis``false`</span><span class="sxs-lookup"><span data-stu-id="992b9-277">`personQuery` set to a value other than `me` and `useContactApis` set to `false`</span></span> | <span data-ttu-id="992b9-278">People.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="992b9-278">People.Read, User.ReadBasic.All</span></span> | <span data-ttu-id="992b9-279">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people)</span><span class="sxs-lookup"><span data-stu-id="992b9-279">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people)</span></span> |
| <span data-ttu-id="992b9-280">`showPresence` установлено `true` и `personQuery` установлено `me`</span><span class="sxs-lookup"><span data-stu-id="992b9-280">`showPresence` set to `true` and `personQuery` set to `me`</span></span> | <span data-ttu-id="992b9-281">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="992b9-281">Presence.Read</span></span> | [<span data-ttu-id="992b9-282">/me/presence</span><span class="sxs-lookup"><span data-stu-id="992b9-282">/me/presence</span></span>](/graph/api/presence-get) |
| <span data-ttu-id="992b9-283">`showPresence`установлено `true` значение, заме- `personQuery``me`</span><span class="sxs-lookup"><span data-stu-id="992b9-283">`showPresence` set to `true` and `personQuery` set to a value other than `me`</span></span> | <span data-ttu-id="992b9-284">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="992b9-284">Presence.Read.All</span></span> | [<span data-ttu-id="992b9-285">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="992b9-285">/users/{id}/presence</span></span>](/graph/api/presence-get) |
| <span data-ttu-id="992b9-286">`personCardInteraction` значение, заме- `PersonCardInteraction.none`</span><span class="sxs-lookup"><span data-stu-id="992b9-286">`personCardInteraction` set to a value other than `PersonCardInteraction.none`</span></span> | <span data-ttu-id="992b9-287">См. [разрешения на карточку человека](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="992b9-287">See [person card permissions](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span></span> | <span data-ttu-id="992b9-288">См. [вызовы API карт персоны](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="992b9-288">See [person card API calls](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span></span> |

## <a name="authentication"></a><span data-ttu-id="992b9-289">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="992b9-289">Authentication</span></span>

<span data-ttu-id="992b9-290">Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="992b9-290">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="992b9-291">Кэш</span><span class="sxs-lookup"><span data-stu-id="992b9-291">Cache</span></span>

|<span data-ttu-id="992b9-292">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="992b9-292">Object store</span></span>|<span data-ttu-id="992b9-293">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="992b9-293">Cached data</span></span>|<span data-ttu-id="992b9-294">Примечания</span><span class="sxs-lookup"><span data-stu-id="992b9-294">Remarks</span></span>|
|---------|-----------|-------|
|`photos`|<span data-ttu-id="992b9-295">Фотография человека</span><span class="sxs-lookup"><span data-stu-id="992b9-295">Person's photo</span></span>|<span data-ttu-id="992b9-296">Используется, `avatarType` когда установлено и `photo` `fetchImage` установлено `true`</span><span class="sxs-lookup"><span data-stu-id="992b9-296">Used, when `avatarType` is set to `photo` and `fetchImage` is set to `true`</span></span>|
|`presence`|<span data-ttu-id="992b9-297">Присутствие человека</span><span class="sxs-lookup"><span data-stu-id="992b9-297">Person's presence</span></span>|<span data-ttu-id="992b9-298">Используется, `showPresence` когда установлено `true`</span><span class="sxs-lookup"><span data-stu-id="992b9-298">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="992b9-299">Сведения о пользователях</span><span class="sxs-lookup"><span data-stu-id="992b9-299">Person's user information</span></span>|

<span data-ttu-id="992b9-300">Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="992b9-300">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="992b9-301">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="992b9-301">Extend for more control</span></span>

<span data-ttu-id="992b9-302">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="992b9-302">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="992b9-303">Метод</span><span class="sxs-lookup"><span data-stu-id="992b9-303">Method</span></span> | <span data-ttu-id="992b9-304">Описание</span><span class="sxs-lookup"><span data-stu-id="992b9-304">Description</span></span> |
| - | - |
| <span data-ttu-id="992b9-305">renderLoading</span><span class="sxs-lookup"><span data-stu-id="992b9-305">renderLoading</span></span> | <span data-ttu-id="992b9-306">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="992b9-306">Renders the loading state.</span></span> |
| <span data-ttu-id="992b9-307">renderNoData</span><span class="sxs-lookup"><span data-stu-id="992b9-307">renderNoData</span></span> | <span data-ttu-id="992b9-308">Отображается, если изображение или данные о пользователе недоступны.</span><span class="sxs-lookup"><span data-stu-id="992b9-308">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="992b9-309">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="992b9-309">renderAvatar</span></span> | <span data-ttu-id="992b9-310">Отображает аватар.</span><span class="sxs-lookup"><span data-stu-id="992b9-310">Renders the avatar.</span></span> |
| <span data-ttu-id="992b9-311">renderDetails</span><span class="sxs-lookup"><span data-stu-id="992b9-311">renderDetails</span></span> | <span data-ttu-id="992b9-312">Отображает сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="992b9-312">Renders the person details part.</span></span> |
