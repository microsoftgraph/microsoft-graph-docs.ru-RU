---
title: Компонент пользователя в Microsoft Graph Toolkit
description: Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, имени и/или адреса электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: cfe5f6b97c35c2704def8c4879522268cc8cc91e
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660041"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="02454-103">Компонент пользователя в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="02454-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="02454-104">Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, адреса электронной почты и любых других сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="02454-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="02454-105">Кроме того, в компоненте пользователя используется [mgt-person-card](./person-card.md) для отображения карточки всплывающего окна с дополнительной информации о пользователе.</span><span class="sxs-lookup"><span data-stu-id="02454-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="02454-106">Дополнительные сведения см. в разделе [Карточка пользователя](#person-card).</span><span class="sxs-lookup"><span data-stu-id="02454-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="02454-107">Пример</span><span class="sxs-lookup"><span data-stu-id="02454-107">Example</span></span>

<span data-ttu-id="02454-108">В приведенном далее примере показан пользователь, использующий компонент `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="02454-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="02454-109">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="02454-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="02454-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="02454-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="02454-111">Настройка сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="02454-111">Setting the person details</span></span>

<span data-ttu-id="02454-112">Чтобы задать сведения о пользователе, можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="02454-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="02454-113">Используйте только одно из указанных далее свойств для одного случая:</span><span class="sxs-lookup"><span data-stu-id="02454-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="02454-114">Задайте атрибут `user-id` или свойство `userId`, чтобы получить данные пользователя из Microsoft Graph, используя его идентификатор.</span><span class="sxs-lookup"><span data-stu-id="02454-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="02454-115">Чтобы выполнить поиск определенного пользователя в Microsoft Graph, задайте атрибут `person-query` или свойство `personQuery`.</span><span class="sxs-lookup"><span data-stu-id="02454-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="02454-116">При этом будет выбран первый доступный пользователь и будут получены сведения об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="02454-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="02454-117">Электронная почта лучше всего подходит для того, чтобы найти нужного пользователя, но можно использовать и имя.</span><span class="sxs-lookup"><span data-stu-id="02454-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="02454-118">Задайте атрибут `person-presence` или свойство `personPresence`, чтобы добавить значок присутствия в аватар пользователя вручную.</span><span class="sxs-lookup"><span data-stu-id="02454-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="02454-119">Чтобы определить размер аватара, задайте для атрибута `avatar-size` или свойства `avatarSize` значение `small` или `large`.</span><span class="sxs-lookup"><span data-stu-id="02454-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="02454-120">Это позволяет добавить [правильный значок присутствия](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) в аватар.</span><span class="sxs-lookup"><span data-stu-id="02454-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="02454-121">Чтобы дополнительно настроить размер аватара, вам нужно выбрать соответствующие настраиваемые свойства CSS, указанные далее.</span><span class="sxs-lookup"><span data-stu-id="02454-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="02454-122">Для этого параметра по умолчанию задано значение `auto`, благодаря которому присутствие будет обрабатываться автоматически с учетом свойства `view`.</span><span class="sxs-lookup"><span data-stu-id="02454-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="02454-123">Рекомендуем использовать `small`, если аватар меньше 32 на 32 пикс.</span><span class="sxs-lookup"><span data-stu-id="02454-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="02454-124">Чтобы вручную задать сведения о пользователе, используйте атрибут `person-details` или свойство `personDetails`, как показано в приведенном далее примере.</span><span class="sxs-lookup"><span data-stu-id="02454-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="02454-125">Если изображение не предоставлено, оно будет получено (при наличии).</span><span class="sxs-lookup"><span data-stu-id="02454-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="02454-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="02454-126">Properties</span></span>

<span data-ttu-id="02454-127">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="02454-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="02454-128">Атрибут</span><span class="sxs-lookup"><span data-stu-id="02454-128">Attribute</span></span>       | <span data-ttu-id="02454-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="02454-129">Property</span></span>       | <span data-ttu-id="02454-130">Описание</span><span class="sxs-lookup"><span data-stu-id="02454-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="02454-131">user-id</span><span class="sxs-lookup"><span data-stu-id="02454-131">user-id</span></span>         | <span data-ttu-id="02454-132">userId</span><span class="sxs-lookup"><span data-stu-id="02454-132">userId</span></span>         | <span data-ttu-id="02454-133">Установите идентификатор пользователя, чтобы получить сведения об этом пользователе и его изображение из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="02454-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="02454-134">person-query</span><span class="sxs-lookup"><span data-stu-id="02454-134">person-query</span></span>    | <span data-ttu-id="02454-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="02454-135">personQuery</span></span>    | <span data-ttu-id="02454-136">Чтобы найти пользователя в Microsoft Graph, установите его имя или адрес электронной почты пользователя и получите сведения о первом пользователе и его изображение.</span><span class="sxs-lookup"><span data-stu-id="02454-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="02454-137">person-details</span><span class="sxs-lookup"><span data-stu-id="02454-137">person-details</span></span>  | <span data-ttu-id="02454-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="02454-138">personDetails</span></span>  | <span data-ttu-id="02454-139">Установите объект, представляющий пользователя.</span><span class="sxs-lookup"><span data-stu-id="02454-139">Set to an object representing a person.</span></span> <span data-ttu-id="02454-140">Используется для объекта из ресурсов "люди", "пользователи", "контакты" или "группа".</span><span class="sxs-lookup"><span data-stu-id="02454-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="02454-141">person-image</span><span class="sxs-lookup"><span data-stu-id="02454-141">person-image</span></span>    | <span data-ttu-id="02454-142">personImage</span><span class="sxs-lookup"><span data-stu-id="02454-142">personImage</span></span>    | <span data-ttu-id="02454-143">Задать изображение, которое будет отображаться для пользователя.</span><span class="sxs-lookup"><span data-stu-id="02454-143">Set the image to show for the person.</span></span> |
| <span data-ttu-id="02454-144">person-presence</span><span class="sxs-lookup"><span data-stu-id="02454-144">person-presence</span></span> | <span data-ttu-id="02454-145">personPresence</span><span class="sxs-lookup"><span data-stu-id="02454-145">personPresence</span></span> | <span data-ttu-id="02454-146">Установка присутствия для пользователя.</span><span class="sxs-lookup"><span data-stu-id="02454-146">Set the presence for the person.</span></span> |
| <span data-ttu-id="02454-147">fetch-image</span><span class="sxs-lookup"><span data-stu-id="02454-147">fetch-image</span></span>     | <span data-ttu-id="02454-148">fetchImage</span><span class="sxs-lookup"><span data-stu-id="02454-148">fetchImage</span></span>     | <span data-ttu-id="02454-149">Установите флажок для автоматического получения `personImage` из Microsoft Graph на основе объекта `personDetails`, предоставленного пользователем.</span><span class="sxs-lookup"><span data-stu-id="02454-149">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="02454-150">представление</span><span class="sxs-lookup"><span data-stu-id="02454-150">view</span></span>            | <span data-ttu-id="02454-151">представление</span><span class="sxs-lookup"><span data-stu-id="02454-151">view</span></span>           | <span data-ttu-id="02454-152">Установите, чтобы настроить, как выглядит пользователь.</span><span class="sxs-lookup"><span data-stu-id="02454-152">Set to control how the person is rendered.</span></span> <span data-ttu-id="02454-153">Значение по умолчанию: `avatar`</span><span class="sxs-lookup"><span data-stu-id="02454-153">Default is `avatar`</span></span> <br /> <span data-ttu-id="02454-154">`avatar` — Показывать только аватар</span><span class="sxs-lookup"><span data-stu-id="02454-154">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="02454-155">`oneline` — Показывать аватар и первую строку (`displayName` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="02454-155">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="02454-156">`twolines` — Показывать аватар и две строки текста (`displayName` и `mail` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="02454-156">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="02454-157">line1-property</span><span class="sxs-lookup"><span data-stu-id="02454-157">line1-property</span></span>  | <span data-ttu-id="02454-158">line1Property</span><span class="sxs-lookup"><span data-stu-id="02454-158">line1Property</span></span>  | <span data-ttu-id="02454-159">Задает свойство personDetails для использования для первой строки текста.</span><span class="sxs-lookup"><span data-stu-id="02454-159">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="02454-160">Значение по умолчанию: `displayName`.</span><span class="sxs-lookup"><span data-stu-id="02454-160">Default is `displayName`.</span></span>|
| <span data-ttu-id="02454-161">line2-property</span><span class="sxs-lookup"><span data-stu-id="02454-161">line2-property</span></span>  | <span data-ttu-id="02454-162">line2Property</span><span class="sxs-lookup"><span data-stu-id="02454-162">line2Property</span></span>  | <span data-ttu-id="02454-163">Задает свойство personDetails для использования для второй строки текста.</span><span class="sxs-lookup"><span data-stu-id="02454-163">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="02454-164">Значение по умолчанию: `mail`.</span><span class="sxs-lookup"><span data-stu-id="02454-164">Default is `mail`.</span></span>|
| <span data-ttu-id="02454-165">line3-property</span><span class="sxs-lookup"><span data-stu-id="02454-165">line3-property</span></span>  | <span data-ttu-id="02454-166">line3Property</span><span class="sxs-lookup"><span data-stu-id="02454-166">line3Property</span></span>  | <span data-ttu-id="02454-167">Задает свойство personDetails для использования для третьей строки текста.</span><span class="sxs-lookup"><span data-stu-id="02454-167">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="02454-168">Значение по умолчанию: `jobTitle`.</span><span class="sxs-lookup"><span data-stu-id="02454-168">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="02454-169">show-presence</span><span class="sxs-lookup"><span data-stu-id="02454-169">show-presence</span></span>   | <span data-ttu-id="02454-170">showPresence</span><span class="sxs-lookup"><span data-stu-id="02454-170">showPresence</span></span>   | <span data-ttu-id="02454-171">Установить флажок отображения присутствия пользователя — по умолчанию `false`.</span><span class="sxs-lookup"><span data-stu-id="02454-171">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="02454-172">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="02454-172">CSS custom properties</span></span>

<span data-ttu-id="02454-173">Компонент `mgt-person` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="02454-173">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  
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

<span data-ttu-id="02454-174">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="02454-174">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="02454-175">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="02454-175">Templates</span></span>

<span data-ttu-id="02454-176">Компонент `mgt-person` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="02454-176">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="02454-177">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="02454-177">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="02454-178">Тип данных</span><span class="sxs-lookup"><span data-stu-id="02454-178">Data type</span></span> | <span data-ttu-id="02454-179">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="02454-179">Data context</span></span> | <span data-ttu-id="02454-180">Описание</span><span class="sxs-lookup"><span data-stu-id="02454-180">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="02454-181">загрузка</span><span class="sxs-lookup"><span data-stu-id="02454-181">loading</span></span> | <span data-ttu-id="02454-182">Нет</span><span class="sxs-lookup"><span data-stu-id="02454-182">none</span></span> | <span data-ttu-id="02454-183">Шаблон для отображения состояния загрузки компонента.</span><span class="sxs-lookup"><span data-stu-id="02454-183">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="02454-184">no-data</span><span class="sxs-lookup"><span data-stu-id="02454-184">no-data</span></span> | <span data-ttu-id="02454-185">Нет</span><span class="sxs-lookup"><span data-stu-id="02454-185">none</span></span> | <span data-ttu-id="02454-186">Шаблон для использования, если изображения или данные не доступны.</span><span class="sxs-lookup"><span data-stu-id="02454-186">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="02454-187">default</span><span class="sxs-lookup"><span data-stu-id="02454-187">default</span></span> | <span data-ttu-id="02454-188">пользователь: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="02454-188">person: The person details object</span></span> <br> <span data-ttu-id="02454-189">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="02454-189">`personImage`: The URL of the image</span></span> | <span data-ttu-id="02454-190">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="02454-190">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="02454-191">person-card</span><span class="sxs-lookup"><span data-stu-id="02454-191">person-card</span></span> | <span data-ttu-id="02454-192">пользователь: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="02454-192">person: The person details object</span></span> <br> <span data-ttu-id="02454-193">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="02454-193">`personImage`: The URL of the image</span></span> | <span data-ttu-id="02454-194">Шаблон для обновления карточки mgt-person-card, отображаемой при наведении указателя мыши или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="02454-194">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="02454-195">В следующем примере определяется шаблон для компонента пользователя.</span><span class="sxs-lookup"><span data-stu-id="02454-195">The following example defines a template for the person component.</span></span>

```html
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
```

## <a name="person-card"></a><span data-ttu-id="02454-196">Карточка пользователя</span><span class="sxs-lookup"><span data-stu-id="02454-196">Person card</span></span>

<span data-ttu-id="02454-197">`mgt-person` Компонент может отображаться`mgt-person-card` при либо наведении указателя мыши, либо щелчка мышью.</span><span class="sxs-lookup"><span data-stu-id="02454-197">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="02454-198">Добавьте средство управления на HTML-страницу.</span><span class="sxs-lookup"><span data-stu-id="02454-198">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="02454-199">Атрибут</span><span class="sxs-lookup"><span data-stu-id="02454-199">Attribute</span></span>    |  <span data-ttu-id="02454-200">Свойство</span><span class="sxs-lookup"><span data-stu-id="02454-200">Property</span></span>     | <span data-ttu-id="02454-201">Описание</span><span class="sxs-lookup"><span data-stu-id="02454-201">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="02454-202">person-card</span><span class="sxs-lookup"><span data-stu-id="02454-202">person-card</span></span> | <span data-ttu-id="02454-203">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="02454-203">personCardInteraction</span></span> | <span data-ttu-id="02454-204">Перечисление для определения пользовательского действия, необходимого для активации всплывающей панели — `hover` или `click`.</span><span class="sxs-lookup"><span data-stu-id="02454-204">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="02454-205">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="02454-205">Default value is `none`</span></span> |


<span data-ttu-id="02454-206">Дополнительные сведения о шаблонах, стилях и атрибутах см. в статье [Компонент карточки пользователя](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="02454-206">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="02454-207">Конфигурация глобального компонента</span><span class="sxs-lookup"><span data-stu-id="02454-207">Global component configuration</span></span>

<span data-ttu-id="02454-208">Класс `MgtPerson` предоставляет статический объект `config`, который конфигурирует все компоненты пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="02454-208">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="02454-209">В приведенном ниже примере показано, как использовать объект конфигурации.</span><span class="sxs-lookup"><span data-stu-id="02454-209">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="02454-210">Ниже указаны свойства, доступные в объекте конфигурации.</span><span class="sxs-lookup"><span data-stu-id="02454-210">The following properties are available on the config object.</span></span>

| <span data-ttu-id="02454-211">Свойство</span><span class="sxs-lookup"><span data-stu-id="02454-211">Property</span></span> | <span data-ttu-id="02454-212">Описание</span><span class="sxs-lookup"><span data-stu-id="02454-212">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="02454-213">useContactApis</span><span class="sxs-lookup"><span data-stu-id="02454-213">useContactApis</span></span> | <span data-ttu-id="02454-214">`boolean` — Указывает, может ли компонент пользователя использовать API личных контактов Microsoft Graph для поиска контактных данных и фотографий.</span><span class="sxs-lookup"><span data-stu-id="02454-214">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="02454-215">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="02454-215">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="02454-216">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="02454-216">Microsoft Graph permissions</span></span>

<span data-ttu-id="02454-217">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="02454-217">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="02454-218">Ресурс</span><span class="sxs-lookup"><span data-stu-id="02454-218">Resource</span></span> | <span data-ttu-id="02454-219">Разрешение</span><span class="sxs-lookup"><span data-stu-id="02454-219">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="02454-220">/me</span><span class="sxs-lookup"><span data-stu-id="02454-220">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="02454-221">User.Read</span><span class="sxs-lookup"><span data-stu-id="02454-221">User.Read</span></span>          |
| [<span data-ttu-id="02454-222">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="02454-222">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="02454-223">User.Read</span><span class="sxs-lookup"><span data-stu-id="02454-223">User.Read</span></span>          |
| [<span data-ttu-id="02454-224">/me/people/?$search=</span><span class="sxs-lookup"><span data-stu-id="02454-224">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="02454-225">People.Read</span><span class="sxs-lookup"><span data-stu-id="02454-225">People.Read</span></span>        |
| [<span data-ttu-id="02454-226">me/contacts\*</span><span class="sxs-lookup"><span data-stu-id="02454-226">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="02454-227">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="02454-227">Contacts.Read</span></span>      |
| [<span data-ttu-id="02454-228">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="02454-228">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="02454-229">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="02454-229">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="02454-230">/me/presence</span><span class="sxs-lookup"><span data-stu-id="02454-230">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="02454-231">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="02454-231">Presence.Read</span></span> |
| [<span data-ttu-id="02454-232">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="02454-232">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="02454-233">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="02454-233">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="02454-234">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="02454-234">Authentication</span></span>

<span data-ttu-id="02454-235">Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="02454-235">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="02454-236">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="02454-236">Extend for more control</span></span>

<span data-ttu-id="02454-237">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="02454-237">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="02454-238">Метод</span><span class="sxs-lookup"><span data-stu-id="02454-238">Method</span></span> | <span data-ttu-id="02454-239">Описание</span><span class="sxs-lookup"><span data-stu-id="02454-239">Description</span></span> |
| - | - |
| <span data-ttu-id="02454-240">renderLoading</span><span class="sxs-lookup"><span data-stu-id="02454-240">renderLoading</span></span> | <span data-ttu-id="02454-241">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="02454-241">Renders the loading state.</span></span> |
| <span data-ttu-id="02454-242">renderNoData</span><span class="sxs-lookup"><span data-stu-id="02454-242">renderNoData</span></span> | <span data-ttu-id="02454-243">Отображается, если изображение или данные о пользователе недоступны.</span><span class="sxs-lookup"><span data-stu-id="02454-243">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="02454-244">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="02454-244">renderAvatar</span></span> | <span data-ttu-id="02454-245">Отображает аватар.</span><span class="sxs-lookup"><span data-stu-id="02454-245">Renders the avatar.</span></span> |
| <span data-ttu-id="02454-246">renderDetails</span><span class="sxs-lookup"><span data-stu-id="02454-246">renderDetails</span></span> | <span data-ttu-id="02454-247">Отображает сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="02454-247">Renders the person details part.</span></span> |
