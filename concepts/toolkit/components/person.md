---
title: Компонент пользователя в Microsoft Graph Toolkit
description: Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, имени и/или адреса электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 7f35b5c1a3ef764995d319e9e603489b50a1fe2c
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082050"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="31fce-103">Компонент пользователя в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="31fce-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="31fce-104">Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, адреса электронной почты и любых других сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="31fce-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="31fce-105">Кроме того, в компоненте пользователя используется [mgt-person-card](./person-card.md) для отображения карточки всплывающего окна с дополнительной информации о пользователе.</span><span class="sxs-lookup"><span data-stu-id="31fce-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="31fce-106">Дополнительные сведения см. в разделе [Карточка пользователя](#person-card).</span><span class="sxs-lookup"><span data-stu-id="31fce-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="31fce-107">Пример</span><span class="sxs-lookup"><span data-stu-id="31fce-107">Example</span></span>

<span data-ttu-id="31fce-108">В приведенном далее примере показан пользователь, использующий компонент `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="31fce-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="31fce-109">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="31fce-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="31fce-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="31fce-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="31fce-111">Настройка сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="31fce-111">Setting the person details</span></span>

<span data-ttu-id="31fce-112">Чтобы задать сведения о пользователе, можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="31fce-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="31fce-113">Используйте только одно из указанных далее свойств для одного случая:</span><span class="sxs-lookup"><span data-stu-id="31fce-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="31fce-114">Задайте атрибут `user-id` или свойство `userId`, чтобы получить данные пользователя из Microsoft Graph, используя его идентификатор.</span><span class="sxs-lookup"><span data-stu-id="31fce-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="31fce-115">Чтобы выполнить поиск определенного пользователя в Microsoft Graph, задайте атрибут `person-query` или свойство `personQuery`.</span><span class="sxs-lookup"><span data-stu-id="31fce-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="31fce-116">При этом будет выбран первый доступный пользователь и будут получены сведения об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="31fce-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="31fce-117">Электронная почта лучше всего подходит для того, чтобы найти нужного пользователя, но можно использовать и имя.</span><span class="sxs-lookup"><span data-stu-id="31fce-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="31fce-118">Задайте атрибут `person-presence` или свойство `personPresence`, чтобы добавить значок присутствия в аватар пользователя вручную.</span><span class="sxs-lookup"><span data-stu-id="31fce-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="31fce-119">Чтобы определить размер аватара, задайте для атрибута `avatar-size` или свойства `avatarSize` значение `small` или `large`.</span><span class="sxs-lookup"><span data-stu-id="31fce-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="31fce-120">Это позволяет добавить [правильный значок присутствия](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) в аватар.</span><span class="sxs-lookup"><span data-stu-id="31fce-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="31fce-121">Чтобы дополнительно настроить размер аватара, вам нужно выбрать соответствующие настраиваемые свойства CSS, указанные далее.</span><span class="sxs-lookup"><span data-stu-id="31fce-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="31fce-122">Для этого параметра по умолчанию задано значение `auto`, благодаря которому присутствие будет обрабатываться автоматически с учетом свойства `view`.</span><span class="sxs-lookup"><span data-stu-id="31fce-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="31fce-123">Рекомендуем использовать `small`, если аватар меньше 32 на 32 пикс.</span><span class="sxs-lookup"><span data-stu-id="31fce-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="31fce-124">Чтобы вручную задать сведения о пользователе, используйте атрибут `person-details` или свойство `personDetails`, как показано в приведенном далее примере.</span><span class="sxs-lookup"><span data-stu-id="31fce-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="31fce-125">Если изображение не предоставлено, оно будет получено (при наличии).</span><span class="sxs-lookup"><span data-stu-id="31fce-125">If no image is provided, one will be fetched (if available).</span></span>

* <span data-ttu-id="31fce-126">По умолчанию компонент пользователя запрашивает только стандартный набор свойств Graph [Майкрософт.](/graph/api/user-get?&tabs=http#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="31fce-126">By default, the person component will only request the standard Microsoft Graph user set of [properties](/graph/api/user-get?&tabs=http#optional-query-parameters).</span></span> <span data-ttu-id="31fce-127">Чтобы запросить дополнительные свойства, объявите их в качестве любой части `line(x)Property` .</span><span class="sxs-lookup"><span data-stu-id="31fce-127">In order to request additional properties, declare them as any part of the `line(x)Property`.</span></span> 


## <a name="properties"></a><span data-ttu-id="31fce-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="31fce-128">Properties</span></span>

<span data-ttu-id="31fce-129">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="31fce-129">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="31fce-130">Атрибут</span><span class="sxs-lookup"><span data-stu-id="31fce-130">Attribute</span></span>       | <span data-ttu-id="31fce-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="31fce-131">Property</span></span>       | <span data-ttu-id="31fce-132">Описание</span><span class="sxs-lookup"><span data-stu-id="31fce-132">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="31fce-133">user-id</span><span class="sxs-lookup"><span data-stu-id="31fce-133">user-id</span></span>         | <span data-ttu-id="31fce-134">userId</span><span class="sxs-lookup"><span data-stu-id="31fce-134">userId</span></span>         | <span data-ttu-id="31fce-135">Установите идентификатор пользователя, чтобы получить сведения об этом пользователе и его изображение из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="31fce-135">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="31fce-136">person-query</span><span class="sxs-lookup"><span data-stu-id="31fce-136">person-query</span></span>    | <span data-ttu-id="31fce-137">personQuery</span><span class="sxs-lookup"><span data-stu-id="31fce-137">personQuery</span></span>    | <span data-ttu-id="31fce-138">Чтобы найти пользователя в Microsoft Graph, установите его имя или адрес электронной почты пользователя и получите сведения о первом пользователе и его изображение.</span><span class="sxs-lookup"><span data-stu-id="31fce-138">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="31fce-139">person-details</span><span class="sxs-lookup"><span data-stu-id="31fce-139">person-details</span></span>  | <span data-ttu-id="31fce-140">personDetails</span><span class="sxs-lookup"><span data-stu-id="31fce-140">personDetails</span></span>  | <span data-ttu-id="31fce-141">Установите объект, представляющий пользователя.</span><span class="sxs-lookup"><span data-stu-id="31fce-141">Set to an object representing a person.</span></span> <span data-ttu-id="31fce-142">Используется для объекта из ресурсов "люди", "пользователи", "контакты" или "группа".</span><span class="sxs-lookup"><span data-stu-id="31fce-142">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="31fce-143">fallback-details</span><span class="sxs-lookup"><span data-stu-id="31fce-143">fallback-details</span></span>| <span data-ttu-id="31fce-144">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="31fce-144">fallbackDetails</span></span>| <span data-ttu-id="31fce-145">Установите объект, представляющий человека, если в графе не обнаружено пользователя/пользователя/контакта.</span><span class="sxs-lookup"><span data-stu-id="31fce-145">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="31fce-146">person-image</span><span class="sxs-lookup"><span data-stu-id="31fce-146">person-image</span></span>    | <span data-ttu-id="31fce-147">personImage</span><span class="sxs-lookup"><span data-stu-id="31fce-147">personImage</span></span>    | <span data-ttu-id="31fce-148">Задать изображение, которое будет отображаться для пользователя.</span><span class="sxs-lookup"><span data-stu-id="31fce-148">Set the image to show for the person.</span></span> |
| <span data-ttu-id="31fce-149">person-presence</span><span class="sxs-lookup"><span data-stu-id="31fce-149">person-presence</span></span> | <span data-ttu-id="31fce-150">personPresence</span><span class="sxs-lookup"><span data-stu-id="31fce-150">personPresence</span></span> | <span data-ttu-id="31fce-151">Установка присутствия для пользователя.</span><span class="sxs-lookup"><span data-stu-id="31fce-151">Set the presence for the person.</span></span> |
| <span data-ttu-id="31fce-152">fetch-image</span><span class="sxs-lookup"><span data-stu-id="31fce-152">fetch-image</span></span>     | <span data-ttu-id="31fce-153">fetchImage</span><span class="sxs-lookup"><span data-stu-id="31fce-153">fetchImage</span></span>     | <span data-ttu-id="31fce-154">Установите флажок для автоматического получения `personImage` из Microsoft Graph на основе объекта `personDetails`, предоставленного пользователем.</span><span class="sxs-lookup"><span data-stu-id="31fce-154">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="31fce-155">тип аватара</span><span class="sxs-lookup"><span data-stu-id="31fce-155">avatar-type</span></span>     | <span data-ttu-id="31fce-156">avatarType</span><span class="sxs-lookup"><span data-stu-id="31fce-156">avatarType</span></span>     | <span data-ttu-id="31fce-157">Установите или `initials` `photo` отобразить состояние отображения по умолчанию — это фотография.</span><span class="sxs-lookup"><span data-stu-id="31fce-157">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="31fce-158">представление</span><span class="sxs-lookup"><span data-stu-id="31fce-158">view</span></span>            | <span data-ttu-id="31fce-159">представление</span><span class="sxs-lookup"><span data-stu-id="31fce-159">view</span></span>           | <span data-ttu-id="31fce-160">Установите, чтобы настроить, как выглядит пользователь.</span><span class="sxs-lookup"><span data-stu-id="31fce-160">Set to control how the person is rendered.</span></span> <span data-ttu-id="31fce-161">Значение по умолчанию: `avatar`</span><span class="sxs-lookup"><span data-stu-id="31fce-161">Default is `avatar`</span></span> <br /> <span data-ttu-id="31fce-162">`avatar` — Показывать только аватар</span><span class="sxs-lookup"><span data-stu-id="31fce-162">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="31fce-163">`oneline` — Показывать аватар и первую строку (`displayName` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="31fce-163">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="31fce-164">`twolines` — Показывать аватар и две строки текста (`displayName` и `mail` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="31fce-164">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="31fce-165">line1-property</span><span class="sxs-lookup"><span data-stu-id="31fce-165">line1-property</span></span>  | <span data-ttu-id="31fce-166">line1Property</span><span class="sxs-lookup"><span data-stu-id="31fce-166">line1Property</span></span>  | <span data-ttu-id="31fce-167">Задает свойство personDetails для использования для первой строки текста.</span><span class="sxs-lookup"><span data-stu-id="31fce-167">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="31fce-168">Значение по умолчанию: `displayName`.</span><span class="sxs-lookup"><span data-stu-id="31fce-168">Default is `displayName`.</span></span>|
| <span data-ttu-id="31fce-169">line2-property</span><span class="sxs-lookup"><span data-stu-id="31fce-169">line2-property</span></span>  | <span data-ttu-id="31fce-170">line2Property</span><span class="sxs-lookup"><span data-stu-id="31fce-170">line2Property</span></span>  | <span data-ttu-id="31fce-171">Задает свойство personDetails для использования для второй строки текста.</span><span class="sxs-lookup"><span data-stu-id="31fce-171">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="31fce-172">Значение по умолчанию: `mail`.</span><span class="sxs-lookup"><span data-stu-id="31fce-172">Default is `mail`.</span></span>|
| <span data-ttu-id="31fce-173">line3-property</span><span class="sxs-lookup"><span data-stu-id="31fce-173">line3-property</span></span>  | <span data-ttu-id="31fce-174">line3Property</span><span class="sxs-lookup"><span data-stu-id="31fce-174">line3Property</span></span>  | <span data-ttu-id="31fce-175">Задает свойство personDetails для использования для третьей строки текста.</span><span class="sxs-lookup"><span data-stu-id="31fce-175">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="31fce-176">Значение по умолчанию: `jobTitle`.</span><span class="sxs-lookup"><span data-stu-id="31fce-176">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="31fce-177">show-presence</span><span class="sxs-lookup"><span data-stu-id="31fce-177">show-presence</span></span>   | <span data-ttu-id="31fce-178">showPresence</span><span class="sxs-lookup"><span data-stu-id="31fce-178">showPresence</span></span>   | <span data-ttu-id="31fce-179">Установить флажок отображения присутствия пользователя — по умолчанию `false`.</span><span class="sxs-lookup"><span data-stu-id="31fce-179">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="31fce-180">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="31fce-180">CSS custom properties</span></span>

<span data-ttu-id="31fce-181">Компонент `mgt-person` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="31fce-181">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="31fce-182">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="31fce-182">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="31fce-183">События</span><span class="sxs-lookup"><span data-stu-id="31fce-183">Events</span></span>

<span data-ttu-id="31fce-184">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="31fce-184">The following events are fired from the component.</span></span>

| <span data-ttu-id="31fce-185">Событие</span><span class="sxs-lookup"><span data-stu-id="31fce-185">Event</span></span> | <span data-ttu-id="31fce-186">Сведения</span><span class="sxs-lookup"><span data-stu-id="31fce-186">Detail</span></span> | <span data-ttu-id="31fce-187">Описание</span><span class="sxs-lookup"><span data-stu-id="31fce-187">Description</span></span> |
| --- | --- | --- |
| `line1clicked` | <span data-ttu-id="31fce-188">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="31fce-188">The detail contains the respective `person` object</span></span> | <span data-ttu-id="31fce-189">Уволено при нажатии строки 1.</span><span class="sxs-lookup"><span data-stu-id="31fce-189">Fired when line1 is clicked.</span></span> |
| `line2clicked` | <span data-ttu-id="31fce-190">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="31fce-190">The detail contains the respective `person` object</span></span> | <span data-ttu-id="31fce-191">Уволено при нажатии строки2.</span><span class="sxs-lookup"><span data-stu-id="31fce-191">Fired when line2 is clicked.</span></span> |
| `line3clicked` | <span data-ttu-id="31fce-192">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="31fce-192">The detail contains the respective `person` object</span></span> | <span data-ttu-id="31fce-193">Уволено при нажатии строки 3.</span><span class="sxs-lookup"><span data-stu-id="31fce-193">Fired when line3 is clicked.</span></span> |

<span data-ttu-id="31fce-194">Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)</span><span class="sxs-lookup"><span data-stu-id="31fce-194">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="templates"></a><span data-ttu-id="31fce-195">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="31fce-195">Templates</span></span>

<span data-ttu-id="31fce-196">Компонент `mgt-person` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="31fce-196">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="31fce-197">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="31fce-197">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="31fce-198">Тип данных</span><span class="sxs-lookup"><span data-stu-id="31fce-198">Data type</span></span> | <span data-ttu-id="31fce-199">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="31fce-199">Data context</span></span> | <span data-ttu-id="31fce-200">Описание</span><span class="sxs-lookup"><span data-stu-id="31fce-200">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="31fce-201">загрузка</span><span class="sxs-lookup"><span data-stu-id="31fce-201">loading</span></span> | <span data-ttu-id="31fce-202">Нет</span><span class="sxs-lookup"><span data-stu-id="31fce-202">none</span></span> | <span data-ttu-id="31fce-203">Шаблон для отображения состояния загрузки компонента.</span><span class="sxs-lookup"><span data-stu-id="31fce-203">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="31fce-204">no-data</span><span class="sxs-lookup"><span data-stu-id="31fce-204">no-data</span></span> | <span data-ttu-id="31fce-205">Нет</span><span class="sxs-lookup"><span data-stu-id="31fce-205">none</span></span> | <span data-ttu-id="31fce-206">Шаблон для использования, если изображения или данные не доступны.</span><span class="sxs-lookup"><span data-stu-id="31fce-206">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="31fce-207">default</span><span class="sxs-lookup"><span data-stu-id="31fce-207">default</span></span> | <span data-ttu-id="31fce-208">пользователь: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="31fce-208">person: The person details object</span></span> <br> <span data-ttu-id="31fce-209">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="31fce-209">`personImage`: The URL of the image</span></span> <br> <span data-ttu-id="31fce-210">`personPresence`: Объект сведений о присутствии для человека</span><span class="sxs-lookup"><span data-stu-id="31fce-210">`personPresence`: The presence details object for person</span></span>  | <span data-ttu-id="31fce-211">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="31fce-211">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="31fce-212">person-card</span><span class="sxs-lookup"><span data-stu-id="31fce-212">person-card</span></span> | <span data-ttu-id="31fce-213">пользователь: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="31fce-213">person: The person details object</span></span> <br> <span data-ttu-id="31fce-214">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="31fce-214">`personImage`: The URL of the image</span></span> | <span data-ttu-id="31fce-215">Шаблон для обновления карточки mgt-person-card, отображаемой при наведении указателя мыши или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="31fce-215">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="31fce-216">line1</span><span class="sxs-lookup"><span data-stu-id="31fce-216">line1</span></span> | <span data-ttu-id="31fce-217">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="31fce-217">person: The person details object</span></span> | <span data-ttu-id="31fce-218">Шаблон для первой строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="31fce-218">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="31fce-219">line2</span><span class="sxs-lookup"><span data-stu-id="31fce-219">line2</span></span> | <span data-ttu-id="31fce-220">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="31fce-220">person: The person details object</span></span> | <span data-ttu-id="31fce-221">Шаблон для второй строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="31fce-221">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="31fce-222">line3</span><span class="sxs-lookup"><span data-stu-id="31fce-222">line3</span></span> | <span data-ttu-id="31fce-223">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="31fce-223">person: The person details object</span></span> | <span data-ttu-id="31fce-224">Шаблон для третьей строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="31fce-224">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="31fce-225">В следующем примере определяется шаблон для компонента пользователя.</span><span class="sxs-lookup"><span data-stu-id="31fce-225">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="31fce-226">Карточка пользователя</span><span class="sxs-lookup"><span data-stu-id="31fce-226">Person card</span></span>

<span data-ttu-id="31fce-227">`mgt-person` Компонент может отображаться`mgt-person-card` при либо наведении указателя мыши, либо щелчка мышью.</span><span class="sxs-lookup"><span data-stu-id="31fce-227">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="31fce-228">Добавьте средство управления на HTML-страницу.</span><span class="sxs-lookup"><span data-stu-id="31fce-228">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="31fce-229">Атрибут</span><span class="sxs-lookup"><span data-stu-id="31fce-229">Attribute</span></span>    |  <span data-ttu-id="31fce-230">Свойство</span><span class="sxs-lookup"><span data-stu-id="31fce-230">Property</span></span>     | <span data-ttu-id="31fce-231">Описание</span><span class="sxs-lookup"><span data-stu-id="31fce-231">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="31fce-232">person-card</span><span class="sxs-lookup"><span data-stu-id="31fce-232">person-card</span></span> | <span data-ttu-id="31fce-233">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="31fce-233">personCardInteraction</span></span> | <span data-ttu-id="31fce-234">Перечисление для определения пользовательского действия, необходимого для активации всплывающей панели — `hover` или `click`.</span><span class="sxs-lookup"><span data-stu-id="31fce-234">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="31fce-235">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="31fce-235">Default value is `none`</span></span> |


<span data-ttu-id="31fce-236">Дополнительные сведения о шаблонах, стилях и атрибутах см. в статье [Компонент карточки пользователя](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="31fce-236">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="31fce-237">Конфигурация глобального компонента</span><span class="sxs-lookup"><span data-stu-id="31fce-237">Global component configuration</span></span>

<span data-ttu-id="31fce-238">Класс `MgtPerson` предоставляет статический объект `config`, который конфигурирует все компоненты пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="31fce-238">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="31fce-239">В приведенном ниже примере показано, как использовать объект конфигурации.</span><span class="sxs-lookup"><span data-stu-id="31fce-239">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="31fce-240">Ниже указаны свойства, доступные в объекте конфигурации.</span><span class="sxs-lookup"><span data-stu-id="31fce-240">The following properties are available on the config object.</span></span>

| <span data-ttu-id="31fce-241">Свойство</span><span class="sxs-lookup"><span data-stu-id="31fce-241">Property</span></span> | <span data-ttu-id="31fce-242">Описание</span><span class="sxs-lookup"><span data-stu-id="31fce-242">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="31fce-243">useContactApis</span><span class="sxs-lookup"><span data-stu-id="31fce-243">useContactApis</span></span> | <span data-ttu-id="31fce-244">`boolean` — Указывает, может ли компонент пользователя использовать API личных контактов Microsoft Graph для поиска контактных данных и фотографий.</span><span class="sxs-lookup"><span data-stu-id="31fce-244">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="31fce-245">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="31fce-245">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="31fce-246">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="31fce-246">Microsoft Graph permissions</span></span>

<span data-ttu-id="31fce-247">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="31fce-247">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="31fce-248">Настройка</span><span class="sxs-lookup"><span data-stu-id="31fce-248">Configuration</span></span> | <span data-ttu-id="31fce-249">Разрешение</span><span class="sxs-lookup"><span data-stu-id="31fce-249">Permission</span></span> | <span data-ttu-id="31fce-250">API</span><span class="sxs-lookup"><span data-stu-id="31fce-250">API</span></span> |
| ------------- | ---------- | --- |
| <span data-ttu-id="31fce-251">`personDetails` установить без изображения, `fetchImage` установить , установить , `true` извлекаемого `avatarType` человека является контакт и `photo` `useContactApis` установить `true`</span><span class="sxs-lookup"><span data-stu-id="31fce-251">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo`, retrieved person is a contact and `useContactApis` set to `true`</span></span> | <span data-ttu-id="31fce-252">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31fce-252">Contacts.Read</span></span> | [<span data-ttu-id="31fce-253">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="31fce-253">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) |
| <span data-ttu-id="31fce-254">`personDetails` установить без изображения, установить , установить и лицо не является `fetchImage` `true` `avatarType` `photo` контактом или `useContactApis` установлено, чтобы `false`</span><span class="sxs-lookup"><span data-stu-id="31fce-254">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and person is not a contact or `useContactApis` is set to `false`</span></span> | <span data-ttu-id="31fce-255">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="31fce-255">User.ReadBasic.All</span></span> | [<span data-ttu-id="31fce-256">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="31fce-256">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="31fce-257">`personDetails` набор без изображения, `fetchImage` установленный `true` для , `avatarType` заданный пользователем и `photo` указанный по электронной почте</span><span class="sxs-lookup"><span data-stu-id="31fce-257">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and user specified via email</span></span> | <span data-ttu-id="31fce-258">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="31fce-258">User.ReadBasic.All</span></span> | [<span data-ttu-id="31fce-259">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="31fce-259">/users/{id}/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="31fce-260">`personDetails` набор без изображения, `fetchImage` `true` `avatarType` заданный, заданный и `photo` контакт, указанный по электронной почте</span><span class="sxs-lookup"><span data-stu-id="31fce-260">`personDetails` set without image, `fetchImage` set to `true`, `avatarType` set to `photo` and contact specified via email</span></span> | <span data-ttu-id="31fce-261">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31fce-261">Contacts.Read</span></span> | [<span data-ttu-id="31fce-262">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="31fce-262">/me/contacts/\*</span></span>](/graph/api/user-list-contacts) |
| <span data-ttu-id="31fce-263">`userId` set</span><span class="sxs-lookup"><span data-stu-id="31fce-263">`userId` set</span></span> | <span data-ttu-id="31fce-264">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="31fce-264">User.ReadBasic.All</span></span> | [<span data-ttu-id="31fce-265">/users/{id}</span><span class="sxs-lookup"><span data-stu-id="31fce-265">/users/{id}</span></span>](/graph/api/user-list-people) |
| <span data-ttu-id="31fce-266">`personQuery` установлено `me` и `avatarType` установлено `photo`</span><span class="sxs-lookup"><span data-stu-id="31fce-266">`personQuery` set to `me` and `avatarType` set to `photo`</span></span> | <span data-ttu-id="31fce-267">User.Read</span><span class="sxs-lookup"><span data-stu-id="31fce-267">User.Read</span></span> | [<span data-ttu-id="31fce-268">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="31fce-268">/me/photo/$value</span></span>](/graph/api/profilephoto-get) |
| <span data-ttu-id="31fce-269">`personQuery` установлено `me` и `avatarType` установлено что-то другое, чем `photo`</span><span class="sxs-lookup"><span data-stu-id="31fce-269">`personQuery` set to `me` and `avatarType` set to something else than `photo`</span></span> | <span data-ttu-id="31fce-270">User.Read</span><span class="sxs-lookup"><span data-stu-id="31fce-270">User.Read</span></span> | [<span data-ttu-id="31fce-271">/me</span><span class="sxs-lookup"><span data-stu-id="31fce-271">/me</span></span>](/graph/api/user-get) |
| <span data-ttu-id="31fce-272">`personQuery`значение, `me` заме- `useContactApis``true`</span><span class="sxs-lookup"><span data-stu-id="31fce-272">`personQuery` set to a value other than `me` and `useContactApis` set to `true`</span></span> | <span data-ttu-id="31fce-273">People.Read, User.ReadBasic.All, Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="31fce-273">People.Read, User.ReadBasic.All, Contacts.Read</span></span> | <span data-ttu-id="31fce-274">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/ \* ](/graph/api/user-list-contacts)</span><span class="sxs-lookup"><span data-stu-id="31fce-274">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people), [/me/contacts/\*](/graph/api/user-list-contacts)</span></span> |
| <span data-ttu-id="31fce-275">`personQuery`значение, `me` заме- `useContactApis``false`</span><span class="sxs-lookup"><span data-stu-id="31fce-275">`personQuery` set to a value other than `me` and `useContactApis` set to `false`</span></span> | <span data-ttu-id="31fce-276">People.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="31fce-276">People.Read, User.ReadBasic.All</span></span> | <span data-ttu-id="31fce-277">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people)</span><span class="sxs-lookup"><span data-stu-id="31fce-277">[/me/people/?$search=](/graph/api/user-list-people), [/users?$search=](/graph/api/user-list-people)</span></span> |
| <span data-ttu-id="31fce-278">`showPresence` установлено `true` и `personQuery` установлено `me`</span><span class="sxs-lookup"><span data-stu-id="31fce-278">`showPresence` set to `true` and `personQuery` set to `me`</span></span> | <span data-ttu-id="31fce-279">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="31fce-279">Presence.Read</span></span> | [<span data-ttu-id="31fce-280">/me/presence</span><span class="sxs-lookup"><span data-stu-id="31fce-280">/me/presence</span></span>](/graph/api/presence-get) |
| <span data-ttu-id="31fce-281">`showPresence`установлено `true` значение, заме- `personQuery``me`</span><span class="sxs-lookup"><span data-stu-id="31fce-281">`showPresence` set to `true` and `personQuery` set to a value other than `me`</span></span> | <span data-ttu-id="31fce-282">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="31fce-282">Presence.Read.All</span></span> | [<span data-ttu-id="31fce-283">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="31fce-283">/users/{id}/presence</span></span>](/graph/api/presence-get) |
| <span data-ttu-id="31fce-284">`personCardInteraction` значение, заме- `PersonCardInteraction.none`</span><span class="sxs-lookup"><span data-stu-id="31fce-284">`personCardInteraction` set to a value other than `PersonCardInteraction.none`</span></span> | <span data-ttu-id="31fce-285">См. [разрешения на карточку человека](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="31fce-285">See [person card permissions](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span></span> | <span data-ttu-id="31fce-286">См. [вызовы API карт персоны](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span><span class="sxs-lookup"><span data-stu-id="31fce-286">See [person card API calls](/graph/toolkit/components/person-card#microsoft-graph-permissions)</span></span> |

## <a name="authentication"></a><span data-ttu-id="31fce-287">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="31fce-287">Authentication</span></span>

<span data-ttu-id="31fce-288">Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="31fce-288">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="31fce-289">Кэш</span><span class="sxs-lookup"><span data-stu-id="31fce-289">Cache</span></span>

|<span data-ttu-id="31fce-290">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="31fce-290">Object store</span></span>|<span data-ttu-id="31fce-291">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="31fce-291">Cached data</span></span>|<span data-ttu-id="31fce-292">Примечания</span><span class="sxs-lookup"><span data-stu-id="31fce-292">Remarks</span></span>|
|---------|-----------|-------|
|`photos`|<span data-ttu-id="31fce-293">Фотография человека</span><span class="sxs-lookup"><span data-stu-id="31fce-293">Person's photo</span></span>|<span data-ttu-id="31fce-294">Используется, `avatarType` когда установлено и `photo` `fetchImage` установлено `true`</span><span class="sxs-lookup"><span data-stu-id="31fce-294">Used, when `avatarType` is set to `photo` and `fetchImage` is set to `true`</span></span>|
|`presence`|<span data-ttu-id="31fce-295">Присутствие человека</span><span class="sxs-lookup"><span data-stu-id="31fce-295">Person's presence</span></span>|<span data-ttu-id="31fce-296">Используется, `showPresence` когда установлено `true`</span><span class="sxs-lookup"><span data-stu-id="31fce-296">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="31fce-297">Сведения о пользователях</span><span class="sxs-lookup"><span data-stu-id="31fce-297">Person's user information</span></span>|

<span data-ttu-id="31fce-298">Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="31fce-298">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="31fce-299">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="31fce-299">Extend for more control</span></span>

<span data-ttu-id="31fce-300">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="31fce-300">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="31fce-301">Метод</span><span class="sxs-lookup"><span data-stu-id="31fce-301">Method</span></span> | <span data-ttu-id="31fce-302">Описание</span><span class="sxs-lookup"><span data-stu-id="31fce-302">Description</span></span> |
| - | - |
| <span data-ttu-id="31fce-303">renderLoading</span><span class="sxs-lookup"><span data-stu-id="31fce-303">renderLoading</span></span> | <span data-ttu-id="31fce-304">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="31fce-304">Renders the loading state.</span></span> |
| <span data-ttu-id="31fce-305">renderNoData</span><span class="sxs-lookup"><span data-stu-id="31fce-305">renderNoData</span></span> | <span data-ttu-id="31fce-306">Отображается, если изображение или данные о пользователе недоступны.</span><span class="sxs-lookup"><span data-stu-id="31fce-306">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="31fce-307">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="31fce-307">renderAvatar</span></span> | <span data-ttu-id="31fce-308">Отображает аватар.</span><span class="sxs-lookup"><span data-stu-id="31fce-308">Renders the avatar.</span></span> |
| <span data-ttu-id="31fce-309">renderDetails</span><span class="sxs-lookup"><span data-stu-id="31fce-309">renderDetails</span></span> | <span data-ttu-id="31fce-310">Отображает сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="31fce-310">Renders the person details part.</span></span> |
