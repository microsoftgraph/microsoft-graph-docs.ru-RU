---
title: Компонент пользователя в Microsoft Graph Toolkit
description: Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, имени и/или адреса электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 46ba7c780985e71d68fe9270f165292136f2e46b
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579951"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1c7fd-103">Компонент пользователя в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1c7fd-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1c7fd-104">Компонент пользователя используется для отображения пользователя или контакта с помощью его фотографии, адреса электронной почты и любых других сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="1c7fd-105">Кроме того, в компоненте пользователя используется [mgt-person-card](./person-card.md) для отображения карточки всплывающего окна с дополнительной информации о пользователе.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="1c7fd-106">Дополнительные сведения см. в разделе [Карточка пользователя](#person-card).</span><span class="sxs-lookup"><span data-stu-id="1c7fd-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="1c7fd-107">Пример</span><span class="sxs-lookup"><span data-stu-id="1c7fd-107">Example</span></span>

<span data-ttu-id="1c7fd-108">В приведенном далее примере показан пользователь, использующий компонент `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="1c7fd-109">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="1c7fd-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="1c7fd-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="1c7fd-111">Настройка сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="1c7fd-111">Setting the person details</span></span>

<span data-ttu-id="1c7fd-112">Чтобы задать сведения о пользователе, можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="1c7fd-113">Используйте только одно из указанных далее свойств для одного случая:</span><span class="sxs-lookup"><span data-stu-id="1c7fd-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="1c7fd-114">Задайте атрибут `user-id` или свойство `userId`, чтобы получить данные пользователя из Microsoft Graph, используя его идентификатор.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="1c7fd-115">Чтобы выполнить поиск определенного пользователя в Microsoft Graph, задайте атрибут `person-query` или свойство `personQuery`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="1c7fd-116">При этом будет выбран первый доступный пользователь и будут получены сведения об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="1c7fd-117">Электронная почта лучше всего подходит для того, чтобы найти нужного пользователя, но можно использовать и имя.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="1c7fd-118">Задайте атрибут `person-presence` или свойство `personPresence`, чтобы добавить значок присутствия в аватар пользователя вручную.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="1c7fd-119">Чтобы определить размер аватара, задайте для атрибута `avatar-size` или свойства `avatarSize` значение `small` или `large`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="1c7fd-120">Это позволяет добавить [правильный значок присутствия](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) в аватар.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="1c7fd-121">Чтобы дополнительно настроить размер аватара, вам нужно выбрать соответствующие настраиваемые свойства CSS, указанные далее.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="1c7fd-122">Для этого параметра по умолчанию задано значение `auto`, благодаря которому присутствие будет обрабатываться автоматически с учетом свойства `view`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="1c7fd-123">Рекомендуем использовать `small`, если аватар меньше 32 на 32 пикс.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="1c7fd-124">Чтобы вручную задать сведения о пользователе, используйте атрибут `person-details` или свойство `personDetails`, как показано в приведенном далее примере.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="1c7fd-125">Если изображение не предоставлено, оно будет получено (при наличии).</span><span class="sxs-lookup"><span data-stu-id="1c7fd-125">If no image is provided, one will be fetched (if available).</span></span>

* <span data-ttu-id="1c7fd-126">По умолчанию компонент пользователя запрашивает только стандартный набор свойств Graph [Майкрософт.](/graph/api/user-get?&tabs=http#optional-query-parameters)</span><span class="sxs-lookup"><span data-stu-id="1c7fd-126">By default, the person component will only request the standard Microsoft Graph user set of [properties](/graph/api/user-get?&tabs=http#optional-query-parameters).</span></span> <span data-ttu-id="1c7fd-127">Чтобы запросить дополнительные свойства, объявите их в качестве любой части `line(x)Property` .</span><span class="sxs-lookup"><span data-stu-id="1c7fd-127">In order to request additional properties, declare them as any part of the `line(x)Property`.</span></span> 


## <a name="properties"></a><span data-ttu-id="1c7fd-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c7fd-128">Properties</span></span>

<span data-ttu-id="1c7fd-129">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-129">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="1c7fd-130">Атрибут</span><span class="sxs-lookup"><span data-stu-id="1c7fd-130">Attribute</span></span>       | <span data-ttu-id="1c7fd-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c7fd-131">Property</span></span>       | <span data-ttu-id="1c7fd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1c7fd-132">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="1c7fd-133">user-id</span><span class="sxs-lookup"><span data-stu-id="1c7fd-133">user-id</span></span>         | <span data-ttu-id="1c7fd-134">userId</span><span class="sxs-lookup"><span data-stu-id="1c7fd-134">userId</span></span>         | <span data-ttu-id="1c7fd-135">Установите идентификатор пользователя, чтобы получить сведения об этом пользователе и его изображение из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-135">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="1c7fd-136">person-query</span><span class="sxs-lookup"><span data-stu-id="1c7fd-136">person-query</span></span>    | <span data-ttu-id="1c7fd-137">personQuery</span><span class="sxs-lookup"><span data-stu-id="1c7fd-137">personQuery</span></span>    | <span data-ttu-id="1c7fd-138">Чтобы найти пользователя в Microsoft Graph, установите его имя или адрес электронной почты пользователя и получите сведения о первом пользователе и его изображение.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-138">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="1c7fd-139">person-details</span><span class="sxs-lookup"><span data-stu-id="1c7fd-139">person-details</span></span>  | <span data-ttu-id="1c7fd-140">personDetails</span><span class="sxs-lookup"><span data-stu-id="1c7fd-140">personDetails</span></span>  | <span data-ttu-id="1c7fd-141">Установите объект, представляющий пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-141">Set to an object representing a person.</span></span> <span data-ttu-id="1c7fd-142">Используется для объекта из ресурсов "люди", "пользователи", "контакты" или "группа".</span><span class="sxs-lookup"><span data-stu-id="1c7fd-142">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="1c7fd-143">fallback-details</span><span class="sxs-lookup"><span data-stu-id="1c7fd-143">fallback-details</span></span>| <span data-ttu-id="1c7fd-144">fallbackDetails</span><span class="sxs-lookup"><span data-stu-id="1c7fd-144">fallbackDetails</span></span>| <span data-ttu-id="1c7fd-145">Установите объект, представляющий человека, если в графе не обнаружено пользователя/пользователя/контакта.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-145">Set to an object representing a person when no user/person/contact is found in the graph.</span></span>
| <span data-ttu-id="1c7fd-146">person-image</span><span class="sxs-lookup"><span data-stu-id="1c7fd-146">person-image</span></span>    | <span data-ttu-id="1c7fd-147">personImage</span><span class="sxs-lookup"><span data-stu-id="1c7fd-147">personImage</span></span>    | <span data-ttu-id="1c7fd-148">Задать изображение, которое будет отображаться для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-148">Set the image to show for the person.</span></span> |
| <span data-ttu-id="1c7fd-149">person-presence</span><span class="sxs-lookup"><span data-stu-id="1c7fd-149">person-presence</span></span> | <span data-ttu-id="1c7fd-150">personPresence</span><span class="sxs-lookup"><span data-stu-id="1c7fd-150">personPresence</span></span> | <span data-ttu-id="1c7fd-151">Установка присутствия для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-151">Set the presence for the person.</span></span> |
| <span data-ttu-id="1c7fd-152">fetch-image</span><span class="sxs-lookup"><span data-stu-id="1c7fd-152">fetch-image</span></span>     | <span data-ttu-id="1c7fd-153">fetchImage</span><span class="sxs-lookup"><span data-stu-id="1c7fd-153">fetchImage</span></span>     | <span data-ttu-id="1c7fd-154">Установите флажок для автоматического получения `personImage` из Microsoft Graph на основе объекта `personDetails`, предоставленного пользователем.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-154">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="1c7fd-155">тип аватара</span><span class="sxs-lookup"><span data-stu-id="1c7fd-155">avatar-type</span></span>     | <span data-ttu-id="1c7fd-156">avatarType</span><span class="sxs-lookup"><span data-stu-id="1c7fd-156">avatarType</span></span>     | <span data-ttu-id="1c7fd-157">Установите или `initials` `photo` отобразить состояние отображения по умолчанию — это фотография.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-157">Set to `initials` or `photo` to render either display state - default is photo.</span></span> |
| <span data-ttu-id="1c7fd-158">представление</span><span class="sxs-lookup"><span data-stu-id="1c7fd-158">view</span></span>            | <span data-ttu-id="1c7fd-159">представление</span><span class="sxs-lookup"><span data-stu-id="1c7fd-159">view</span></span>           | <span data-ttu-id="1c7fd-160">Установите, чтобы настроить, как выглядит пользователь.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-160">Set to control how the person is rendered.</span></span> <span data-ttu-id="1c7fd-161">Значение по умолчанию: `avatar`</span><span class="sxs-lookup"><span data-stu-id="1c7fd-161">Default is `avatar`</span></span> <br /> <span data-ttu-id="1c7fd-162">`avatar` — Показывать только аватар</span><span class="sxs-lookup"><span data-stu-id="1c7fd-162">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="1c7fd-163">`oneline` — Показывать аватар и первую строку (`displayName` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="1c7fd-163">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="1c7fd-164">`twolines` — Показывать аватар и две строки текста (`displayName` и `mail` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="1c7fd-164">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="1c7fd-165">line1-property</span><span class="sxs-lookup"><span data-stu-id="1c7fd-165">line1-property</span></span>  | <span data-ttu-id="1c7fd-166">line1Property</span><span class="sxs-lookup"><span data-stu-id="1c7fd-166">line1Property</span></span>  | <span data-ttu-id="1c7fd-167">Задает свойство personDetails для использования для первой строки текста.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-167">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="1c7fd-168">Значение по умолчанию: `displayName`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-168">Default is `displayName`.</span></span>|
| <span data-ttu-id="1c7fd-169">line2-property</span><span class="sxs-lookup"><span data-stu-id="1c7fd-169">line2-property</span></span>  | <span data-ttu-id="1c7fd-170">line2Property</span><span class="sxs-lookup"><span data-stu-id="1c7fd-170">line2Property</span></span>  | <span data-ttu-id="1c7fd-171">Задает свойство personDetails для использования для второй строки текста.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-171">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="1c7fd-172">Значение по умолчанию: `mail`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-172">Default is `mail`.</span></span>|
| <span data-ttu-id="1c7fd-173">line3-property</span><span class="sxs-lookup"><span data-stu-id="1c7fd-173">line3-property</span></span>  | <span data-ttu-id="1c7fd-174">line3Property</span><span class="sxs-lookup"><span data-stu-id="1c7fd-174">line3Property</span></span>  | <span data-ttu-id="1c7fd-175">Задает свойство personDetails для использования для третьей строки текста.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-175">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="1c7fd-176">Значение по умолчанию: `jobTitle`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-176">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="1c7fd-177">show-presence</span><span class="sxs-lookup"><span data-stu-id="1c7fd-177">show-presence</span></span>   | <span data-ttu-id="1c7fd-178">showPresence</span><span class="sxs-lookup"><span data-stu-id="1c7fd-178">showPresence</span></span>   | <span data-ttu-id="1c7fd-179">Установить флажок отображения присутствия пользователя — по умолчанию `false`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-179">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="1c7fd-180">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="1c7fd-180">CSS custom properties</span></span>

<span data-ttu-id="1c7fd-181">Компонент `mgt-person` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-181">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="1c7fd-182">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="1c7fd-182">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="events"></a><span data-ttu-id="1c7fd-183">События</span><span class="sxs-lookup"><span data-stu-id="1c7fd-183">Events</span></span>

<span data-ttu-id="1c7fd-184">Из компонента инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-184">The following events are fired from the component.</span></span>

| <span data-ttu-id="1c7fd-185">Событие</span><span class="sxs-lookup"><span data-stu-id="1c7fd-185">Event</span></span> | <span data-ttu-id="1c7fd-186">Сведения</span><span class="sxs-lookup"><span data-stu-id="1c7fd-186">Detail</span></span> | <span data-ttu-id="1c7fd-187">Описание</span><span class="sxs-lookup"><span data-stu-id="1c7fd-187">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1c7fd-188">line1clicked</span><span class="sxs-lookup"><span data-stu-id="1c7fd-188">line1clicked</span></span> | <span data-ttu-id="1c7fd-189">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="1c7fd-189">The detail contains the respective `person` object</span></span> | <span data-ttu-id="1c7fd-190">Уволено при нажатии строки 1.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-190">Fired when line1 is clicked.</span></span> |
| <span data-ttu-id="1c7fd-191">line2clicked</span><span class="sxs-lookup"><span data-stu-id="1c7fd-191">line2clicked</span></span> | <span data-ttu-id="1c7fd-192">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="1c7fd-192">The detail contains the respective `person` object</span></span> | <span data-ttu-id="1c7fd-193">Уволено при нажатии строки2.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-193">Fired when line2 is clicked.</span></span> |
| <span data-ttu-id="1c7fd-194">line3clicked</span><span class="sxs-lookup"><span data-stu-id="1c7fd-194">line3clicked</span></span> | <span data-ttu-id="1c7fd-195">Сведения содержат соответствующий объект `person`</span><span class="sxs-lookup"><span data-stu-id="1c7fd-195">The detail contains the respective `person` object</span></span> | <span data-ttu-id="1c7fd-196">Уволено при нажатии строки 3.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-196">Fired when line3 is clicked.</span></span> |

## <a name="templates"></a><span data-ttu-id="1c7fd-197">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="1c7fd-197">Templates</span></span>

<span data-ttu-id="1c7fd-198">Компонент `mgt-person` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-198">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="1c7fd-199">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и установите для параметра `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-199">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="1c7fd-200">Тип данных</span><span class="sxs-lookup"><span data-stu-id="1c7fd-200">Data type</span></span> | <span data-ttu-id="1c7fd-201">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="1c7fd-201">Data context</span></span> | <span data-ttu-id="1c7fd-202">Описание</span><span class="sxs-lookup"><span data-stu-id="1c7fd-202">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="1c7fd-203">загрузка</span><span class="sxs-lookup"><span data-stu-id="1c7fd-203">loading</span></span> | <span data-ttu-id="1c7fd-204">Нет</span><span class="sxs-lookup"><span data-stu-id="1c7fd-204">none</span></span> | <span data-ttu-id="1c7fd-205">Шаблон для отображения состояния загрузки компонента.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-205">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="1c7fd-206">no-data</span><span class="sxs-lookup"><span data-stu-id="1c7fd-206">no-data</span></span> | <span data-ttu-id="1c7fd-207">Нет</span><span class="sxs-lookup"><span data-stu-id="1c7fd-207">none</span></span> | <span data-ttu-id="1c7fd-208">Шаблон для использования, если изображения или данные не доступны.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-208">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="1c7fd-209">default</span><span class="sxs-lookup"><span data-stu-id="1c7fd-209">default</span></span> | <span data-ttu-id="1c7fd-210">пользователь: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="1c7fd-210">person: The person details object</span></span> <br> <span data-ttu-id="1c7fd-211">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-211">`personImage`: The URL of the image</span></span> <br> <span data-ttu-id="1c7fd-212">`personPresence`: Объект сведений о присутствии для человека</span><span class="sxs-lookup"><span data-stu-id="1c7fd-212">`personPresence`: The presence details object for person</span></span>  | <span data-ttu-id="1c7fd-213">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-213">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="1c7fd-214">person-card</span><span class="sxs-lookup"><span data-stu-id="1c7fd-214">person-card</span></span> | <span data-ttu-id="1c7fd-215">пользователь: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="1c7fd-215">person: The person details object</span></span> <br> <span data-ttu-id="1c7fd-216">`personImage`: URL-адрес изображения.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-216">`personImage`: The URL of the image</span></span> | <span data-ttu-id="1c7fd-217">Шаблон для обновления карточки mgt-person-card, отображаемой при наведении указателя мыши или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-217">The template to update the mgt-person-card displayed on hover or click.</span></span> |
| <span data-ttu-id="1c7fd-218">line1</span><span class="sxs-lookup"><span data-stu-id="1c7fd-218">line1</span></span> | <span data-ttu-id="1c7fd-219">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="1c7fd-219">person: The person details object</span></span> | <span data-ttu-id="1c7fd-220">Шаблон для первой строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-220">The template for the first line of person metadata.</span></span> |
| <span data-ttu-id="1c7fd-221">line2</span><span class="sxs-lookup"><span data-stu-id="1c7fd-221">line2</span></span> | <span data-ttu-id="1c7fd-222">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="1c7fd-222">person: The person details object</span></span> | <span data-ttu-id="1c7fd-223">Шаблон для второй строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-223">The template for the second line of person metadata.</span></span> |
| <span data-ttu-id="1c7fd-224">line3</span><span class="sxs-lookup"><span data-stu-id="1c7fd-224">line3</span></span> | <span data-ttu-id="1c7fd-225">person: объект сведений о пользователе</span><span class="sxs-lookup"><span data-stu-id="1c7fd-225">person: The person details object</span></span> | <span data-ttu-id="1c7fd-226">Шаблон для третьей строки метаданных человека.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-226">The template for the third line of person metadata.</span></span> |

<span data-ttu-id="1c7fd-227">В следующем примере определяется шаблон для компонента пользователя.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-227">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="1c7fd-228">Карточка пользователя</span><span class="sxs-lookup"><span data-stu-id="1c7fd-228">Person card</span></span>

<span data-ttu-id="1c7fd-229">`mgt-person` Компонент может отображаться`mgt-person-card` при либо наведении указателя мыши, либо щелчка мышью.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-229">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="1c7fd-230">Добавьте средство управления на HTML-страницу.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-230">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="1c7fd-231">Атрибут</span><span class="sxs-lookup"><span data-stu-id="1c7fd-231">Attribute</span></span>    |  <span data-ttu-id="1c7fd-232">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c7fd-232">Property</span></span>     | <span data-ttu-id="1c7fd-233">Описание</span><span class="sxs-lookup"><span data-stu-id="1c7fd-233">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="1c7fd-234">person-card</span><span class="sxs-lookup"><span data-stu-id="1c7fd-234">person-card</span></span> | <span data-ttu-id="1c7fd-235">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="1c7fd-235">personCardInteraction</span></span> | <span data-ttu-id="1c7fd-236">Перечисление для определения пользовательского действия, необходимого для активации всплывающей панели — `hover` или `click`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-236">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="1c7fd-237">Значение по умолчанию: `none`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-237">Default value is `none`</span></span> |


<span data-ttu-id="1c7fd-238">Дополнительные сведения о шаблонах, стилях и атрибутах см. в статье [Компонент карточки пользователя](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="1c7fd-238">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="1c7fd-239">Конфигурация глобального компонента</span><span class="sxs-lookup"><span data-stu-id="1c7fd-239">Global component configuration</span></span>

<span data-ttu-id="1c7fd-240">Класс `MgtPerson` предоставляет статический объект `config`, который конфигурирует все компоненты пользователя в приложении.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-240">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="1c7fd-241">В приведенном ниже примере показано, как использовать объект конфигурации.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-241">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="1c7fd-242">Ниже указаны свойства, доступные в объекте конфигурации.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-242">The following properties are available on the config object.</span></span>

| <span data-ttu-id="1c7fd-243">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c7fd-243">Property</span></span> | <span data-ttu-id="1c7fd-244">Описание</span><span class="sxs-lookup"><span data-stu-id="1c7fd-244">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="1c7fd-245">useContactApis</span><span class="sxs-lookup"><span data-stu-id="1c7fd-245">useContactApis</span></span> | <span data-ttu-id="1c7fd-246">`boolean` — Указывает, может ли компонент пользователя использовать API личных контактов Microsoft Graph для поиска контактных данных и фотографий.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-246">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="1c7fd-247">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-247">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="1c7fd-248">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1c7fd-248">Microsoft Graph permissions</span></span>

<span data-ttu-id="1c7fd-249">Этот элемент управления использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-249">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="1c7fd-250">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1c7fd-250">Resource</span></span> | <span data-ttu-id="1c7fd-251">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1c7fd-251">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="1c7fd-252">/me</span><span class="sxs-lookup"><span data-stu-id="1c7fd-252">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="1c7fd-253">User.Read</span><span class="sxs-lookup"><span data-stu-id="1c7fd-253">User.Read</span></span>          |
| [<span data-ttu-id="1c7fd-254">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="1c7fd-254">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="1c7fd-255">User.Read</span><span class="sxs-lookup"><span data-stu-id="1c7fd-255">User.Read</span></span>          |
| [<span data-ttu-id="1c7fd-256">/me/people/?$search=</span><span class="sxs-lookup"><span data-stu-id="1c7fd-256">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="1c7fd-257">People.Read</span><span class="sxs-lookup"><span data-stu-id="1c7fd-257">People.Read</span></span>        |
| [<span data-ttu-id="1c7fd-258">me/contacts\*</span><span class="sxs-lookup"><span data-stu-id="1c7fd-258">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="1c7fd-259">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1c7fd-259">Contacts.Read</span></span>      |
| [<span data-ttu-id="1c7fd-260">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="1c7fd-260">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="1c7fd-261">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1c7fd-261">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="1c7fd-262">/me/presence</span><span class="sxs-lookup"><span data-stu-id="1c7fd-262">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="1c7fd-263">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="1c7fd-263">Presence.Read</span></span> |
| [<span data-ttu-id="1c7fd-264">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="1c7fd-264">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="1c7fd-265">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c7fd-265">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="1c7fd-266">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="1c7fd-266">Authentication</span></span>

<span data-ttu-id="1c7fd-267">Для получения требуемых данных в средстве управления используется глобальный поставщик проверки подлинности, указанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="1c7fd-267">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="cache"></a><span data-ttu-id="1c7fd-268">Кэш</span><span class="sxs-lookup"><span data-stu-id="1c7fd-268">Cache</span></span>

|<span data-ttu-id="1c7fd-269">Хранилище объектов</span><span class="sxs-lookup"><span data-stu-id="1c7fd-269">Object store</span></span>|<span data-ttu-id="1c7fd-270">Кэшные данные</span><span class="sxs-lookup"><span data-stu-id="1c7fd-270">Cached data</span></span>|<span data-ttu-id="1c7fd-271">Примечания</span><span class="sxs-lookup"><span data-stu-id="1c7fd-271">Remarks</span></span>|
|---------|-----------|-------|
|`photos`|<span data-ttu-id="1c7fd-272">Фотография человека</span><span class="sxs-lookup"><span data-stu-id="1c7fd-272">Person's photo</span></span>|<span data-ttu-id="1c7fd-273">Используется, `avatarType` когда установлено и `photo` `fetchImage` установлено `true`</span><span class="sxs-lookup"><span data-stu-id="1c7fd-273">Used, when `avatarType` is set to `photo` and `fetchImage` is set to `true`</span></span>|
|`presence`|<span data-ttu-id="1c7fd-274">Присутствие человека</span><span class="sxs-lookup"><span data-stu-id="1c7fd-274">Person's presence</span></span>|<span data-ttu-id="1c7fd-275">Используется, `showPresence` когда установлено `true`</span><span class="sxs-lookup"><span data-stu-id="1c7fd-275">Used, when `showPresence` is set to `true`</span></span>|
|`users`|<span data-ttu-id="1c7fd-276">Сведения о пользователях</span><span class="sxs-lookup"><span data-stu-id="1c7fd-276">Person's user information</span></span>|

<span data-ttu-id="1c7fd-277">Дополнительные сведения о настройке кэша см. в [caching.](../customize-components/cache.md)</span><span class="sxs-lookup"><span data-stu-id="1c7fd-277">See [Caching](../customize-components/cache.md) for more details on how to configure the cache.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="1c7fd-278">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="1c7fd-278">Extend for more control</span></span>

<span data-ttu-id="1c7fd-279">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected render*` для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-279">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="1c7fd-280">Метод</span><span class="sxs-lookup"><span data-stu-id="1c7fd-280">Method</span></span> | <span data-ttu-id="1c7fd-281">Описание</span><span class="sxs-lookup"><span data-stu-id="1c7fd-281">Description</span></span> |
| - | - |
| <span data-ttu-id="1c7fd-282">renderLoading</span><span class="sxs-lookup"><span data-stu-id="1c7fd-282">renderLoading</span></span> | <span data-ttu-id="1c7fd-283">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-283">Renders the loading state.</span></span> |
| <span data-ttu-id="1c7fd-284">renderNoData</span><span class="sxs-lookup"><span data-stu-id="1c7fd-284">renderNoData</span></span> | <span data-ttu-id="1c7fd-285">Отображается, если изображение или данные о пользователе недоступны.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-285">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="1c7fd-286">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="1c7fd-286">renderAvatar</span></span> | <span data-ttu-id="1c7fd-287">Отображает аватар.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-287">Renders the avatar.</span></span> |
| <span data-ttu-id="1c7fd-288">renderDetails</span><span class="sxs-lookup"><span data-stu-id="1c7fd-288">renderDetails</span></span> | <span data-ttu-id="1c7fd-289">Отображает сведения о пользователе.</span><span class="sxs-lookup"><span data-stu-id="1c7fd-289">Renders the person details part.</span></span> |
