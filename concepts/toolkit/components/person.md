---
title: Компонент Person в наборе инструментов Microsoft Graph
description: Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e08e98a29ab454dca546d0fda34b8292ad97bf2d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681881"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="58dc4-103">Компонент Person в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="58dc4-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="58dc4-104">Компонент Person используется для отображения человека или контакта с помощью фотографии, имени, адреса электронной почты или других сведений о человеке.</span><span class="sxs-lookup"><span data-stu-id="58dc4-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="58dc4-105">Кроме того, для отображения всплывающей карточки с дополнительными сведениями о пользователе в компоненте Person используется [карточка упр](./person-card.md) ./Person.</span><span class="sxs-lookup"><span data-stu-id="58dc4-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="58dc4-106">Дополнительные сведения можно найти в разделе [карточка пользователя](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="58dc4-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="58dc4-107">Пример</span><span class="sxs-lookup"><span data-stu-id="58dc4-107">Example</span></span>

<span data-ttu-id="58dc4-108">В приведенном ниже примере отображается пользователь, использующий `mgt-person` компонент.</span><span class="sxs-lookup"><span data-stu-id="58dc4-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="58dc4-109">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="58dc4-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="58dc4-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="58dc4-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="58dc4-111">Настройка сведений о лице</span><span class="sxs-lookup"><span data-stu-id="58dc4-111">Setting the person details</span></span>

<span data-ttu-id="58dc4-112">Для задания сведений о лице можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="58dc4-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="58dc4-113">Используйте только одно из следующих свойств для каждого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="58dc4-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="58dc4-114">Задайте `user-id` атрибут или `userId` свойство, чтобы получить пользователя из Microsoft Graph с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="58dc4-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="58dc4-115">Задайте `person-query` атрибут или `personQuery` свойство для поиска определенного пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58dc4-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="58dc4-116">Он выбирает первого пользователя, который будет доступен, и извлекает сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="58dc4-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="58dc4-117">Электронная почта обеспечивает наилучшее обращение к нужному человеку, но имя также работает.</span><span class="sxs-lookup"><span data-stu-id="58dc4-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="58dc4-118">Задайте `person-presence` атрибут или `personPresence` свойство, чтобы добавить значок присутствия для аватара вручную.</span><span class="sxs-lookup"><span data-stu-id="58dc4-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="58dc4-119">Присвойте `avatar-size` атрибуту или `avatarSize` свойству значение, `small` `large` определяющее размер аватара.</span><span class="sxs-lookup"><span data-stu-id="58dc4-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="58dc4-120">Это помогает добавить [соответствующий значок присутствия](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) в Аватар.</span><span class="sxs-lookup"><span data-stu-id="58dc4-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="58dc4-121">Для дальнейшей настройки размера аватара вам потребуется выбрать соответствующие настраиваемые свойства CSS, показанные ниже.</span><span class="sxs-lookup"><span data-stu-id="58dc4-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="58dc4-122">По умолчанию задано значение, `auto` которое автоматически решает, как отображать сведения о присутствии на основе `view` Свойства.</span><span class="sxs-lookup"><span data-stu-id="58dc4-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="58dc4-123">Мы рекомендуем использовать `small` , если ваш аватар меньше, чем интервалами по 32, интервалами по 32.</span><span class="sxs-lookup"><span data-stu-id="58dc4-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="58dc4-124">Используйте `person-details` атрибут или `personDetails` свойство, чтобы вручную задать сведения о лице, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="58dc4-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="58dc4-125">Если изображение не указано, выбирается один из них (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="58dc4-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="58dc4-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="58dc4-126">Properties</span></span>

<span data-ttu-id="58dc4-127">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="58dc4-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="58dc4-128">Атрибут</span><span class="sxs-lookup"><span data-stu-id="58dc4-128">Attribute</span></span>       | <span data-ttu-id="58dc4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="58dc4-129">Property</span></span>       | <span data-ttu-id="58dc4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="58dc4-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="58dc4-131">User — ID</span><span class="sxs-lookup"><span data-stu-id="58dc4-131">user-id</span></span>         | <span data-ttu-id="58dc4-132">userId</span><span class="sxs-lookup"><span data-stu-id="58dc4-132">userId</span></span>         | <span data-ttu-id="58dc4-133">Задает идентификатор пользователя для получения сведений о пользователе и изображения из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58dc4-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="58dc4-134">Person — запрос</span><span class="sxs-lookup"><span data-stu-id="58dc4-134">person-query</span></span>    | <span data-ttu-id="58dc4-135">персонкуери</span><span class="sxs-lookup"><span data-stu-id="58dc4-135">personQuery</span></span>    | <span data-ttu-id="58dc4-136">Задайте имя или адрес электронной почты человека, который будет выполнять поиск человека в Microsoft Graph, и извлекают сведения и изображения первого пользователя.</span><span class="sxs-lookup"><span data-stu-id="58dc4-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="58dc4-137">Person — сведения</span><span class="sxs-lookup"><span data-stu-id="58dc4-137">person-details</span></span>  | <span data-ttu-id="58dc4-138">персондетаилс</span><span class="sxs-lookup"><span data-stu-id="58dc4-138">personDetails</span></span>  | <span data-ttu-id="58dc4-139">Задайте объект, представляющий человека.</span><span class="sxs-lookup"><span data-stu-id="58dc4-139">Set to an object representing a person.</span></span> <span data-ttu-id="58dc4-140">Работает с объектом из списка люди, пользователи, контакты или группа ресурсов.</span><span class="sxs-lookup"><span data-stu-id="58dc4-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="58dc4-141">Person — изображение</span><span class="sxs-lookup"><span data-stu-id="58dc4-141">person-image</span></span>    | <span data-ttu-id="58dc4-142">персонимаже</span><span class="sxs-lookup"><span data-stu-id="58dc4-142">personImage</span></span>    | <span data-ttu-id="58dc4-143">Задайте изображение, которое будет отображаться для пользователя.</span><span class="sxs-lookup"><span data-stu-id="58dc4-143">Set the image to show for the person.</span></span> |
| <span data-ttu-id="58dc4-144">Person — присутствие</span><span class="sxs-lookup"><span data-stu-id="58dc4-144">person-presence</span></span> | <span data-ttu-id="58dc4-145">персонпресенце</span><span class="sxs-lookup"><span data-stu-id="58dc4-145">personPresence</span></span> | <span data-ttu-id="58dc4-146">Задайте сведения о присутствии для пользователя.</span><span class="sxs-lookup"><span data-stu-id="58dc4-146">Set the presence for the person.</span></span> |
| <span data-ttu-id="58dc4-147">Извлечение изображения</span><span class="sxs-lookup"><span data-stu-id="58dc4-147">fetch-image</span></span>     | <span data-ttu-id="58dc4-148">фетчимаже</span><span class="sxs-lookup"><span data-stu-id="58dc4-148">fetchImage</span></span>     | <span data-ttu-id="58dc4-149">Установите флаг для `personImage` автоматического извлечения из Microsoft Graph на основе `personDetails` объекта, предоставленного пользователем.</span><span class="sxs-lookup"><span data-stu-id="58dc4-149">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="58dc4-150">view</span><span class="sxs-lookup"><span data-stu-id="58dc4-150">view</span></span>            | <span data-ttu-id="58dc4-151">view</span><span class="sxs-lookup"><span data-stu-id="58dc4-151">view</span></span>           | <span data-ttu-id="58dc4-152">Настройка управления отображением человека.</span><span class="sxs-lookup"><span data-stu-id="58dc4-152">Set to control how the person is rendered.</span></span> <span data-ttu-id="58dc4-153">Значение по умолчанию:`avatar`</span><span class="sxs-lookup"><span data-stu-id="58dc4-153">Default is `avatar`</span></span> <br /> <span data-ttu-id="58dc4-154">`avatar`— Показывать только аватар</span><span class="sxs-lookup"><span data-stu-id="58dc4-154">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="58dc4-155">`oneline`-показывать аватар и первую строку (по `displayName` умолчанию)</span><span class="sxs-lookup"><span data-stu-id="58dc4-155">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="58dc4-156">`twolines`-Показать аватар и две строки текста (по `displayName` `mail` умолчанию)</span><span class="sxs-lookup"><span data-stu-id="58dc4-156">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="58dc4-157">строка1 — Property</span><span class="sxs-lookup"><span data-stu-id="58dc4-157">line1-property</span></span>  | <span data-ttu-id="58dc4-158">line1Property</span><span class="sxs-lookup"><span data-stu-id="58dc4-158">line1Property</span></span>  | <span data-ttu-id="58dc4-159">Задает свойство Персондетаилс, которое будет использоваться для первой строки текста.</span><span class="sxs-lookup"><span data-stu-id="58dc4-159">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="58dc4-160">Значение по умолчанию: `displayName`.</span><span class="sxs-lookup"><span data-stu-id="58dc4-160">Default is `displayName`.</span></span>|
| <span data-ttu-id="58dc4-161">строка2 — свойство</span><span class="sxs-lookup"><span data-stu-id="58dc4-161">line2-property</span></span>  | <span data-ttu-id="58dc4-162">line2Property</span><span class="sxs-lookup"><span data-stu-id="58dc4-162">line2Property</span></span>  | <span data-ttu-id="58dc4-163">Задает свойство Персондетаилс для использования во второй строке текста.</span><span class="sxs-lookup"><span data-stu-id="58dc4-163">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="58dc4-164">Значение по умолчанию: `mail`.</span><span class="sxs-lookup"><span data-stu-id="58dc4-164">Default is `mail`.</span></span>|
| <span data-ttu-id="58dc4-165">Показать — присутствие</span><span class="sxs-lookup"><span data-stu-id="58dc4-165">show-presence</span></span>   | <span data-ttu-id="58dc4-166">шовпресенце</span><span class="sxs-lookup"><span data-stu-id="58dc4-166">showPresence</span></span>   | <span data-ttu-id="58dc4-167">Установите флаг для отображения сведений о присутствии пользователя — значение по умолчанию `false` .</span><span class="sxs-lookup"><span data-stu-id="58dc4-167">Set flag to display person presence - default is `false`.</span></span>|
| <span data-ttu-id="58dc4-168">Show (имя)</span><span class="sxs-lookup"><span data-stu-id="58dc4-168">show-name</span></span>       | <span data-ttu-id="58dc4-169">шовнаме</span><span class="sxs-lookup"><span data-stu-id="58dc4-169">showName</span></span>       | <span data-ttu-id="58dc4-170">**УСТАРЕВШее использование `view` .**</span><span class="sxs-lookup"><span data-stu-id="58dc4-170">**DEPRECATED - use `view`.**</span></span>  <span data-ttu-id="58dc4-171">Установите флаг для отображения отображаемого имени пользователя — значение по умолчанию — `false` .</span><span class="sxs-lookup"><span data-stu-id="58dc4-171">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="58dc4-172">Show — email</span><span class="sxs-lookup"><span data-stu-id="58dc4-172">show-email</span></span>      | <span data-ttu-id="58dc4-173">шовемаил</span><span class="sxs-lookup"><span data-stu-id="58dc4-173">showEmail</span></span>      | <span data-ttu-id="58dc4-174">**УСТАРЕВШее использование `view` .**</span><span class="sxs-lookup"><span data-stu-id="58dc4-174">**DEPRECATED - use `view`.**</span></span> <span data-ttu-id="58dc4-175">Установите флаг для отображения электронной почты пользователя — значение по умолчанию — `false` .</span><span class="sxs-lookup"><span data-stu-id="58dc4-175">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="58dc4-176">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="58dc4-176">CSS custom properties</span></span>

<span data-ttu-id="58dc4-177">`mgt-person`Компонент определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="58dc4-177">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size: 48px;
  --avatar-border: 0;
  --avatar-border-radius: 50%;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-family: 'Segoe UI';
  --font-size: 14px;
  --font-weight: 500;
  --color: black;
  --text-transform: none;
  --line2-font-size: 12px;
  --line2-font-weight: 400;
  --line2-color: black;
  --line2-text-transform: none;
  --details-spacing: 12px;
}
```

<span data-ttu-id="58dc4-178">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="58dc4-178">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="58dc4-179">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="58dc4-179">Templates</span></span>

<span data-ttu-id="58dc4-180">`mgt-person`Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="58dc4-180">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="58dc4-181">Чтобы указать шаблон, включите элемент в `<template>` компонент и задайте `data-type` для него одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="58dc4-181">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="58dc4-182">Тип данных</span><span class="sxs-lookup"><span data-stu-id="58dc4-182">Data type</span></span> | <span data-ttu-id="58dc4-183">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="58dc4-183">Data context</span></span> | <span data-ttu-id="58dc4-184">Description</span><span class="sxs-lookup"><span data-stu-id="58dc4-184">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="58dc4-185">загрузки</span><span class="sxs-lookup"><span data-stu-id="58dc4-185">loading</span></span> | <span data-ttu-id="58dc4-186">Нет</span><span class="sxs-lookup"><span data-stu-id="58dc4-186">none</span></span> | <span data-ttu-id="58dc4-187">Шаблон, который будет отображаться, пока компонент находится в состоянии лаодинг.</span><span class="sxs-lookup"><span data-stu-id="58dc4-187">The template to render while the component is in a laoding state.</span></span> |
| <span data-ttu-id="58dc4-188">нет данных</span><span class="sxs-lookup"><span data-stu-id="58dc4-188">no-data</span></span> | <span data-ttu-id="58dc4-189">Нет</span><span class="sxs-lookup"><span data-stu-id="58dc4-189">none</span></span> | <span data-ttu-id="58dc4-190">Шаблон для отображения при отсутствии изображения или данных, доступных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="58dc4-190">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="58dc4-191">Значение  по умолчанию</span><span class="sxs-lookup"><span data-stu-id="58dc4-191">default</span></span> | <span data-ttu-id="58dc4-192">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="58dc4-192">person: The person details object</span></span> <br> <span data-ttu-id="58dc4-193">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="58dc4-193">`personImage`: The URL of the image</span></span> | <span data-ttu-id="58dc4-194">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="58dc4-194">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="58dc4-195">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="58dc4-195">person-card</span></span> | <span data-ttu-id="58dc4-196">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="58dc4-196">person: The person details object</span></span> <br> <span data-ttu-id="58dc4-197">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="58dc4-197">`personImage`: The URL of the image</span></span> | <span data-ttu-id="58dc4-198">Шаблон для обновления карточки упр. Person, отображаемой при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="58dc4-198">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="58dc4-199">В следующем примере определяется шаблон для компонента Person.</span><span class="sxs-lookup"><span data-stu-id="58dc4-199">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="58dc4-200">Карточка пользователя</span><span class="sxs-lookup"><span data-stu-id="58dc4-200">Person Card</span></span>

<span data-ttu-id="58dc4-201">`mgt-person`Компонент может отображать элемент `mgt-person-card` при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="58dc4-201">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="58dc4-202">Добавление элемента управления на HTML-страницу</span><span class="sxs-lookup"><span data-stu-id="58dc4-202">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="58dc4-203">Атрибут</span><span class="sxs-lookup"><span data-stu-id="58dc4-203">Attribute</span></span>    |  <span data-ttu-id="58dc4-204">Свойство</span><span class="sxs-lookup"><span data-stu-id="58dc4-204">Property</span></span>     | <span data-ttu-id="58dc4-205">Описание</span><span class="sxs-lookup"><span data-stu-id="58dc4-205">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="58dc4-206">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="58dc4-206">person-card</span></span> | <span data-ttu-id="58dc4-207">персонкардинтерактион</span><span class="sxs-lookup"><span data-stu-id="58dc4-207">personCardInteraction</span></span> | <span data-ttu-id="58dc4-208">Перечисление для определения действия пользователя, необходимого для активации всплывающей панели `hover` `click` .</span><span class="sxs-lookup"><span data-stu-id="58dc4-208">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="58dc4-209">Значение по умолчанию:`none`</span><span class="sxs-lookup"><span data-stu-id="58dc4-209">Default value is `none`</span></span> |


<span data-ttu-id="58dc4-210">Для получения дополнительных сведений о шаблонах, стилях и атрибутах обратитесь к [компоненту карточки сотрудника](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="58dc4-210">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="58dc4-211">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="58dc4-211">Microsoft Graph permissions</span></span>

<span data-ttu-id="58dc4-212">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58dc4-212">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="58dc4-213">Resource</span><span class="sxs-lookup"><span data-stu-id="58dc4-213">Resource</span></span>                                                                                                    | <span data-ttu-id="58dc4-214">Permission</span><span class="sxs-lookup"><span data-stu-id="58dc4-214">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="58dc4-215">/ме</span><span class="sxs-lookup"><span data-stu-id="58dc4-215">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="58dc4-216">User.Read</span><span class="sxs-lookup"><span data-stu-id="58dc4-216">User.Read</span></span>          |
| [<span data-ttu-id="58dc4-217">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="58dc4-217">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="58dc4-218">User.Read</span><span class="sxs-lookup"><span data-stu-id="58dc4-218">User.Read</span></span>          |
| [<span data-ttu-id="58dc4-219">/ме/Пеопле/? $search =</span><span class="sxs-lookup"><span data-stu-id="58dc4-219">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="58dc4-220">People.Read</span><span class="sxs-lookup"><span data-stu-id="58dc4-220">People.Read</span></span>        |
| [<span data-ttu-id="58dc4-221">/ме/контактс/\*</span><span class="sxs-lookup"><span data-stu-id="58dc4-221">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="58dc4-222">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="58dc4-222">Contacts.Read</span></span>      |
| [<span data-ttu-id="58dc4-223">/усерс/{ИД}/фото/$value</span><span class="sxs-lookup"><span data-stu-id="58dc4-223">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="58dc4-224">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="58dc4-224">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="58dc4-225">/ме/пресенце</span><span class="sxs-lookup"><span data-stu-id="58dc4-225">/me/presence</span></span>](/graph/api/presence-get?view=graph-rest-beta)                | <span data-ttu-id="58dc4-226">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="58dc4-226">Presence.Read</span></span> |
| [<span data-ttu-id="58dc4-227">/усерс/{ид}/пресенце</span><span class="sxs-lookup"><span data-stu-id="58dc4-227">/users/{id}/presence</span></span>](/graph/api/presence-get?view=graph-rest-beta)        | <span data-ttu-id="58dc4-228">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="58dc4-228">Presence.Read.All</span></span> |

> <span data-ttu-id="58dc4-229">**Примечание:** чтобы получить доступ к `*/photo/$value` ресурсам для личных учетных записей Майкрософт, используйте конечную точку бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="58dc4-229">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="58dc4-230">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="58dc4-230">Authentication</span></span>

<span data-ttu-id="58dc4-231">Для извлечения необходимых данных элемент управления использует глобальную проверку подлинности, описанную в [документации по проверке подлинности](./../providers.md) .</span><span class="sxs-lookup"><span data-stu-id="58dc4-231">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="58dc4-232">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="58dc4-232">Extend for more control</span></span>

<span data-ttu-id="58dc4-233">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет несколько `protected render*` способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="58dc4-233">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="58dc4-234">Метод</span><span class="sxs-lookup"><span data-stu-id="58dc4-234">Method</span></span> | <span data-ttu-id="58dc4-235">Описание</span><span class="sxs-lookup"><span data-stu-id="58dc4-235">Description</span></span> |
| - | - |
| <span data-ttu-id="58dc4-236">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="58dc4-236">renderLoading</span></span> | <span data-ttu-id="58dc4-237">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="58dc4-237">Renders the loading state.</span></span> |
| <span data-ttu-id="58dc4-238">рендернодата</span><span class="sxs-lookup"><span data-stu-id="58dc4-238">renderNoData</span></span> | <span data-ttu-id="58dc4-239">Отрисовывает, когда нет доступных изображений или данных о пользователях.</span><span class="sxs-lookup"><span data-stu-id="58dc4-239">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="58dc4-240">рендераватар</span><span class="sxs-lookup"><span data-stu-id="58dc4-240">renderAvatar</span></span> | <span data-ttu-id="58dc4-241">Отрисовывает аватар.</span><span class="sxs-lookup"><span data-stu-id="58dc4-241">Renders the avatar.</span></span> |
| <span data-ttu-id="58dc4-242">рендердетаилс</span><span class="sxs-lookup"><span data-stu-id="58dc4-242">renderDetails</span></span> | <span data-ttu-id="58dc4-243">Отрисовывает часть сведений о лице.</span><span class="sxs-lookup"><span data-stu-id="58dc4-243">Renders the person details part.</span></span> |
