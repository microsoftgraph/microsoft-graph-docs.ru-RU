---
title: Компонент person в microsoft Graph набор средств
description: Компонент person используется для отображения человека или контакта с помощью его фотографии, имени и/или адреса электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: cfe5f6b97c35c2704def8c4879522268cc8cc91e
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660041"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ebb92-103">Компонент person в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="ebb92-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ebb92-104">Компонент лица используется для отображения человека или контакта с помощью его фотографии, имени, адреса электронной почты или любых других сведений о человеке.</span><span class="sxs-lookup"><span data-stu-id="ebb92-104">The person component is used to display a person or contact by using their photo, name, email address, or any other person details.</span></span>

<span data-ttu-id="ebb92-105">Компонент пользователя также использует [карточку mgt-person для](./person-card.md) отображения карточки с дополнительными сведениями о пользователе.</span><span class="sxs-lookup"><span data-stu-id="ebb92-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="ebb92-106">Подробные сведения см. в [разделе "Карточка человека".](#person-card)</span><span class="sxs-lookup"><span data-stu-id="ebb92-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="ebb92-107">Пример</span><span class="sxs-lookup"><span data-stu-id="ebb92-107">Example</span></span>

<span data-ttu-id="ebb92-108">В следующем примере отображается человек, использующий `mgt-person` компонент.</span><span class="sxs-lookup"><span data-stu-id="ebb92-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="ebb92-109">С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="ebb92-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="ebb92-110">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="ebb92-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="ebb92-111">Настройка сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="ebb92-111">Setting the person details</span></span>

<span data-ttu-id="ebb92-112">Чтобы установить сведения о человеке, можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="ebb92-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="ebb92-113">Используйте только одно из следующих свойств для каждого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="ebb92-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="ebb92-114">Установите атрибут или свойство для получения пользователя `user-id` из Microsoft Graph по его `userId` ИД.</span><span class="sxs-lookup"><span data-stu-id="ebb92-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="ebb92-115">Установите атрибут `person-query` или свойство для поиска в Microsoft Graph для `personQuery` заданного человека.</span><span class="sxs-lookup"><span data-stu-id="ebb92-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="ebb92-116">Он выберет первого доступного человека и получит сведения о нем.</span><span class="sxs-lookup"><span data-stu-id="ebb92-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="ebb92-117">Сообщение электронной почты лучше всего работает для запроса нужного человека, но имя также работает.</span><span class="sxs-lookup"><span data-stu-id="ebb92-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="ebb92-118">Установите атрибут `person-presence` или `personPresence` свойство, чтобы добавить эмблему присутствия для аватара пользователя вручную.</span><span class="sxs-lookup"><span data-stu-id="ebb92-118">Set the `person-presence` attribute or `personPresence` property to add a presence badge to person avatar manually.</span></span>

* <span data-ttu-id="ebb92-119">Установите для `avatar-size` атрибута `avatarSize` или свойства или `small` `large` определите размер аватара.</span><span class="sxs-lookup"><span data-stu-id="ebb92-119">Set the `avatar-size` attribute or `avatarSize` property to `small` or `large` to determine the size of avatar.</span></span> <span data-ttu-id="ebb92-120">Это помогает добавить правильный [индикатор присутствия в](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) аватар.</span><span class="sxs-lookup"><span data-stu-id="ebb92-120">This helps add the [correct presence badge](https://mgt.dev/?path=/story/components-mgt-person--person-presence-display-all) to avatar.</span></span> <span data-ttu-id="ebb92-121">Вам потребуется выбрать правильные соответствующие настраиваемые свойства CSS, показанные ниже, чтобы дополнительно настроить размер аватара.</span><span class="sxs-lookup"><span data-stu-id="ebb92-121">You will need to choose the correct corresponding css custom properties shown below to further customize avatar size.</span></span> <span data-ttu-id="ebb92-122">По умолчанию устанавливается значение, которое автоматически определяет, как отрисовка присутствия на основе `auto` `view` свойства.</span><span class="sxs-lookup"><span data-stu-id="ebb92-122">By default, the value is set to `auto` which will automatically decide how to render the presence based on the `view` property.</span></span> <span data-ttu-id="ebb92-123">Рекомендуется использовать, если размер вашего аватара меньше `small` 32px на 32px.</span><span class="sxs-lookup"><span data-stu-id="ebb92-123">We recommend using `small` if your avatar is smaller than 32px by 32px.</span></span> 

* <span data-ttu-id="ebb92-124">Используйте атрибут или свойство, чтобы вручную установить сведения о `person-details` `personDetails` человеке, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="ebb92-124">Use the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        mail: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="ebb92-125">Если изображение не предоставлено, он будет извлечен (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="ebb92-125">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="ebb92-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="ebb92-126">Properties</span></span>

<span data-ttu-id="ebb92-127">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="ebb92-127">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="ebb92-128">Атрибут</span><span class="sxs-lookup"><span data-stu-id="ebb92-128">Attribute</span></span>       | <span data-ttu-id="ebb92-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebb92-129">Property</span></span>       | <span data-ttu-id="ebb92-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb92-130">Description</span></span>                                                   |
| -----------     | ----------     | ------------------------------------------------------------- |
| <span data-ttu-id="ebb92-131">user-id</span><span class="sxs-lookup"><span data-stu-id="ebb92-131">user-id</span></span>         | <span data-ttu-id="ebb92-132">userId</span><span class="sxs-lookup"><span data-stu-id="ebb92-132">userId</span></span>         | <span data-ttu-id="ebb92-133">Установите для ид пользователя извлечение сведений и изображения этого пользователя из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ebb92-133">Set to a user id to fetch that user's details and image from Microsoft Graph.</span></span>|
| <span data-ttu-id="ebb92-134">person-query</span><span class="sxs-lookup"><span data-stu-id="ebb92-134">person-query</span></span>    | <span data-ttu-id="ebb92-135">personQuery</span><span class="sxs-lookup"><span data-stu-id="ebb92-135">personQuery</span></span>    | <span data-ttu-id="ebb92-136">Запишите имя или сообщение электронной почты человека для поиска человека в Microsoft Graph и получения сведений и изображения первого человека.</span><span class="sxs-lookup"><span data-stu-id="ebb92-136">Set to a name or email of a person to search for a person in Microsoft Graph and fetch the first person's details and image.</span></span>|
| <span data-ttu-id="ebb92-137">person-details</span><span class="sxs-lookup"><span data-stu-id="ebb92-137">person-details</span></span>  | <span data-ttu-id="ebb92-138">personDetails</span><span class="sxs-lookup"><span data-stu-id="ebb92-138">personDetails</span></span>  | <span data-ttu-id="ebb92-139">Установите объект, представляющий человека.</span><span class="sxs-lookup"><span data-stu-id="ebb92-139">Set to an object representing a person.</span></span> <span data-ttu-id="ebb92-140">Работает с объектом из людей, пользователей, контактов или групп, ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ebb92-140">Works with object from the people, users, contacts, or group, resources.</span></span> |
| <span data-ttu-id="ebb92-141">person-image</span><span class="sxs-lookup"><span data-stu-id="ebb92-141">person-image</span></span>    | <span data-ttu-id="ebb92-142">personImage</span><span class="sxs-lookup"><span data-stu-id="ebb92-142">personImage</span></span>    | <span data-ttu-id="ebb92-143">Закажите изображение, которое будет показываться для этого человека.</span><span class="sxs-lookup"><span data-stu-id="ebb92-143">Set the image to show for the person.</span></span> |
| <span data-ttu-id="ebb92-144">person-presence</span><span class="sxs-lookup"><span data-stu-id="ebb92-144">person-presence</span></span> | <span data-ttu-id="ebb92-145">personPresence</span><span class="sxs-lookup"><span data-stu-id="ebb92-145">personPresence</span></span> | <span data-ttu-id="ebb92-146">Установите присутствие для человека.</span><span class="sxs-lookup"><span data-stu-id="ebb92-146">Set the presence for the person.</span></span> |
| <span data-ttu-id="ebb92-147">fetch-image</span><span class="sxs-lookup"><span data-stu-id="ebb92-147">fetch-image</span></span>     | <span data-ttu-id="ebb92-148">fetchImage</span><span class="sxs-lookup"><span data-stu-id="ebb92-148">fetchImage</span></span>     | <span data-ttu-id="ebb92-149">Установите флаг для автоматического извлечения из Microsoft Graph на основе `personImage` `personDetails` объекта, предоставленного пользователем.</span><span class="sxs-lookup"><span data-stu-id="ebb92-149">Set flag to fetch `personImage` automatically from Microsoft Graph based on the `personDetails` object provided by the user.</span></span> |
| <span data-ttu-id="ebb92-150">view</span><span class="sxs-lookup"><span data-stu-id="ebb92-150">view</span></span>            | <span data-ttu-id="ebb92-151">view</span><span class="sxs-lookup"><span data-stu-id="ebb92-151">view</span></span>           | <span data-ttu-id="ebb92-152">Установите для управления отрисовки человека.</span><span class="sxs-lookup"><span data-stu-id="ebb92-152">Set to control how the person is rendered.</span></span> <span data-ttu-id="ebb92-153">Значение по умолчанию: `avatar`</span><span class="sxs-lookup"><span data-stu-id="ebb92-153">Default is `avatar`</span></span> <br /> <span data-ttu-id="ebb92-154">`avatar` — показывать только аватар</span><span class="sxs-lookup"><span data-stu-id="ebb92-154">`avatar` - show only avatar</span></span> <br /> <span data-ttu-id="ebb92-155">`oneline` - показать аватар и первую строку ( `displayName` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="ebb92-155">`oneline` - show avatar and first line (`displayName` by default)</span></span> <br /> <span data-ttu-id="ebb92-156">`twolines` - показать аватар и две строки текста ( `displayName` и `mail` по умолчанию)</span><span class="sxs-lookup"><span data-stu-id="ebb92-156">`twolines` - show avatar and two lines of text (`displayName` and `mail` by default)</span></span>|
| <span data-ttu-id="ebb92-157">line1-property</span><span class="sxs-lookup"><span data-stu-id="ebb92-157">line1-property</span></span>  | <span data-ttu-id="ebb92-158">line1Property</span><span class="sxs-lookup"><span data-stu-id="ebb92-158">line1Property</span></span>  | <span data-ttu-id="ebb92-159">Задает свойство personDetails, используемого для первой строки текста.</span><span class="sxs-lookup"><span data-stu-id="ebb92-159">Sets the property of the personDetails to use for the first line of text.</span></span> <span data-ttu-id="ebb92-160">Значение по умолчанию: `displayName`.</span><span class="sxs-lookup"><span data-stu-id="ebb92-160">Default is `displayName`.</span></span>|
| <span data-ttu-id="ebb92-161">line2-property</span><span class="sxs-lookup"><span data-stu-id="ebb92-161">line2-property</span></span>  | <span data-ttu-id="ebb92-162">line2Property</span><span class="sxs-lookup"><span data-stu-id="ebb92-162">line2Property</span></span>  | <span data-ttu-id="ebb92-163">Задает свойство personDetails, используемого для второй строки текста.</span><span class="sxs-lookup"><span data-stu-id="ebb92-163">Sets the property of the personDetails to use for the second line of text.</span></span> <span data-ttu-id="ebb92-164">Значение по умолчанию: `mail`.</span><span class="sxs-lookup"><span data-stu-id="ebb92-164">Default is `mail`.</span></span>|
| <span data-ttu-id="ebb92-165">line3-property</span><span class="sxs-lookup"><span data-stu-id="ebb92-165">line3-property</span></span>  | <span data-ttu-id="ebb92-166">line3Property</span><span class="sxs-lookup"><span data-stu-id="ebb92-166">line3Property</span></span>  | <span data-ttu-id="ebb92-167">Задает свойство personDetails, используемого для третьей строки текста.</span><span class="sxs-lookup"><span data-stu-id="ebb92-167">Sets the property of the personDetails to use for the third line of text.</span></span> <span data-ttu-id="ebb92-168">Значение по умолчанию: `jobTitle`.</span><span class="sxs-lookup"><span data-stu-id="ebb92-168">Default is `jobTitle`.</span></span>|
| <span data-ttu-id="ebb92-169">show-presence</span><span class="sxs-lookup"><span data-stu-id="ebb92-169">show-presence</span></span>   | <span data-ttu-id="ebb92-170">showPresence</span><span class="sxs-lookup"><span data-stu-id="ebb92-170">showPresence</span></span>   | <span data-ttu-id="ebb92-171">Установите флаг для отображения присутствия человека — значение по `false` умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ebb92-171">Set flag to display person presence - default is `false`.</span></span>|

## <a name="css-custom-properties"></a><span data-ttu-id="ebb92-172">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="ebb92-172">CSS custom properties</span></span>

<span data-ttu-id="ebb92-173">Компонент `mgt-person` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="ebb92-173">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="ebb92-174">Дополнительные узнать см. [в компонентах стиля.](../customize-components/style.md)</span><span class="sxs-lookup"><span data-stu-id="ebb92-174">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="ebb92-175">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="ebb92-175">Templates</span></span>

<span data-ttu-id="ebb92-176">Компонент `mgt-person` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="ebb92-176">The `mgt-person` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="ebb92-177">Чтобы указать шаблон, включив элемент в компонент и заключив в него одно `<template>` `data-type` из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="ebb92-177">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="ebb92-178">Тип данных</span><span class="sxs-lookup"><span data-stu-id="ebb92-178">Data type</span></span> | <span data-ttu-id="ebb92-179">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="ebb92-179">Data context</span></span> | <span data-ttu-id="ebb92-180">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb92-180">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="ebb92-181">loading</span><span class="sxs-lookup"><span data-stu-id="ebb92-181">loading</span></span> | <span data-ttu-id="ebb92-182">Нет</span><span class="sxs-lookup"><span data-stu-id="ebb92-182">none</span></span> | <span data-ttu-id="ebb92-183">Шаблон для отрисовки, когда компонент находится в состоянии загрузки.</span><span class="sxs-lookup"><span data-stu-id="ebb92-183">The template to render while the component is in a loading state.</span></span> |
| <span data-ttu-id="ebb92-184">no-data</span><span class="sxs-lookup"><span data-stu-id="ebb92-184">no-data</span></span> | <span data-ttu-id="ebb92-185">Нет</span><span class="sxs-lookup"><span data-stu-id="ebb92-185">none</span></span> | <span data-ttu-id="ebb92-186">Шаблон, который необходимо отрисовки, если изображение или данные человека недоступны.</span><span class="sxs-lookup"><span data-stu-id="ebb92-186">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="ebb92-187">default</span><span class="sxs-lookup"><span data-stu-id="ebb92-187">default</span></span> | <span data-ttu-id="ebb92-188">person: объект сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="ebb92-188">person: The person details object</span></span> <br> <span data-ttu-id="ebb92-189">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="ebb92-189">`personImage`: The URL of the image</span></span> | <span data-ttu-id="ebb92-190">Шаблон по умолчанию заменяет весь компонент на собственный.</span><span class="sxs-lookup"><span data-stu-id="ebb92-190">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="ebb92-191">person-card</span><span class="sxs-lookup"><span data-stu-id="ebb92-191">person-card</span></span> | <span data-ttu-id="ebb92-192">person: объект сведений о человеке</span><span class="sxs-lookup"><span data-stu-id="ebb92-192">person: The person details object</span></span> <br> <span data-ttu-id="ebb92-193">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="ebb92-193">`personImage`: The URL of the image</span></span> | <span data-ttu-id="ebb92-194">Шаблон для обновления карточки mgt-person, отображаемой при наведении или щелчке.</span><span class="sxs-lookup"><span data-stu-id="ebb92-194">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="ebb92-195">В следующем примере определяется шаблон для компонента person.</span><span class="sxs-lookup"><span data-stu-id="ebb92-195">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="ebb92-196">Карточка человека</span><span class="sxs-lookup"><span data-stu-id="ebb92-196">Person card</span></span>

<span data-ttu-id="ebb92-197">Компонент `mgt-person` может показываться при `mgt-person-card` наведении или нажатии кнопки мыши.</span><span class="sxs-lookup"><span data-stu-id="ebb92-197">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="ebb92-198">Добавление элементов управления на HTML-страницу</span><span class="sxs-lookup"><span data-stu-id="ebb92-198">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="ebb92-199">Атрибут</span><span class="sxs-lookup"><span data-stu-id="ebb92-199">Attribute</span></span>    |  <span data-ttu-id="ebb92-200">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebb92-200">Property</span></span>     | <span data-ttu-id="ebb92-201">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb92-201">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="ebb92-202">person-card</span><span class="sxs-lookup"><span data-stu-id="ebb92-202">person-card</span></span> | <span data-ttu-id="ebb92-203">personCardInteraction</span><span class="sxs-lookup"><span data-stu-id="ebb92-203">personCardInteraction</span></span> | <span data-ttu-id="ebb92-204">Enumeration to determine user action necessary to activate flyout panel - `hover` or `click` .</span><span class="sxs-lookup"><span data-stu-id="ebb92-204">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="ebb92-205">Значение по умолчанию: `none`</span><span class="sxs-lookup"><span data-stu-id="ebb92-205">Default value is `none`</span></span> |


<span data-ttu-id="ebb92-206">Дополнительные сведения о шаблонах, стилях и атрибутах см. в компоненте [карточки человека.](./person-card.md)</span><span class="sxs-lookup"><span data-stu-id="ebb92-206">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="global-component-configuration"></a><span data-ttu-id="ebb92-207">Глобальная конфигурация компонентов</span><span class="sxs-lookup"><span data-stu-id="ebb92-207">Global component configuration</span></span>

<span data-ttu-id="ebb92-208">Класс `MgtPerson` предоставляет статический `config` объект, который настраивает все компоненты person в приложении.</span><span class="sxs-lookup"><span data-stu-id="ebb92-208">The `MgtPerson` class exposes a static `config` object that configures all person components in the application.</span></span>

<span data-ttu-id="ebb92-209">В следующем примере показано, как использовать объект config.</span><span class="sxs-lookup"><span data-stu-id="ebb92-209">The following example shows how to use the config object.</span></span>

```ts
import { MgtPerson } from `@microsoft/mgt`;

MgtPerson.config.useContactApis = false;
```

<span data-ttu-id="ebb92-210">Для объекта config доступны следующие свойства.</span><span class="sxs-lookup"><span data-stu-id="ebb92-210">The following properties are available on the config object.</span></span>

| <span data-ttu-id="ebb92-211">Свойство</span><span class="sxs-lookup"><span data-stu-id="ebb92-211">Property</span></span> | <span data-ttu-id="ebb92-212">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb92-212">Description</span></span> |
| ------------ | ------------- |
| <span data-ttu-id="ebb92-213">useContactApis</span><span class="sxs-lookup"><span data-stu-id="ebb92-213">useContactApis</span></span> | <span data-ttu-id="ebb92-214">`boolean` - Указывает, может ли компонент лица использовать API личных контактов Microsoft Graph для поиска контактных данных и фотографий.</span><span class="sxs-lookup"><span data-stu-id="ebb92-214">`boolean` - Indicates whether the person component can use the Microsoft Graph personal contacts API to search for contact details and photos.</span></span> <span data-ttu-id="ebb92-215">Значение по умолчанию: `true`.</span><span class="sxs-lookup"><span data-stu-id="ebb92-215">Default value is `true`.</span></span>  |

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="ebb92-216">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ebb92-216">Microsoft Graph permissions</span></span>

<span data-ttu-id="ebb92-217">Этот контроль использует следующие API Microsoft Graph и разрешения.</span><span class="sxs-lookup"><span data-stu-id="ebb92-217">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="ebb92-218">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ebb92-218">Resource</span></span> | <span data-ttu-id="ebb92-219">Разрешение</span><span class="sxs-lookup"><span data-stu-id="ebb92-219">Permission</span></span>     |
| -| - |
| [<span data-ttu-id="ebb92-220">/me</span><span class="sxs-lookup"><span data-stu-id="ebb92-220">/me</span></span>](/graph/api/user-get)                              | <span data-ttu-id="ebb92-221">User.Read</span><span class="sxs-lookup"><span data-stu-id="ebb92-221">User.Read</span></span>          |
| [<span data-ttu-id="ebb92-222">/me/photo/$value</span><span class="sxs-lookup"><span data-stu-id="ebb92-222">/me/photo/$value</span></span>](/graph/api/profilephoto-get)        | <span data-ttu-id="ebb92-223">User.Read</span><span class="sxs-lookup"><span data-stu-id="ebb92-223">User.Read</span></span>          |
| [<span data-ttu-id="ebb92-224">/me/people/?$search=</span><span class="sxs-lookup"><span data-stu-id="ebb92-224">/me/people/?$search=</span></span>](/graph/api/user-list-people)     | <span data-ttu-id="ebb92-225">People.Read</span><span class="sxs-lookup"><span data-stu-id="ebb92-225">People.Read</span></span>        |
| [<span data-ttu-id="ebb92-226">/me/contacts/\*</span><span class="sxs-lookup"><span data-stu-id="ebb92-226">/me/contacts/\*</span></span>](/graph/api/user-list-contacts&tabs=cs) | <span data-ttu-id="ebb92-227">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="ebb92-227">Contacts.Read</span></span>      |
| [<span data-ttu-id="ebb92-228">/users/{id}/photo/$value</span><span class="sxs-lookup"><span data-stu-id="ebb92-228">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people) | <span data-ttu-id="ebb92-229">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="ebb92-229">User.ReadBasic.All</span></span> |
| [<span data-ttu-id="ebb92-230">/me/presence</span><span class="sxs-lookup"><span data-stu-id="ebb92-230">/me/presence</span></span>](/graph/api/presence-get)                | <span data-ttu-id="ebb92-231">Presence.Read</span><span class="sxs-lookup"><span data-stu-id="ebb92-231">Presence.Read</span></span> |
| [<span data-ttu-id="ebb92-232">/users/{id}/presence</span><span class="sxs-lookup"><span data-stu-id="ebb92-232">/users/{id}/presence</span></span>](/graph/api/presence-get)        | <span data-ttu-id="ebb92-233">Presence.Read.All</span><span class="sxs-lookup"><span data-stu-id="ebb92-233">Presence.Read.All</span></span> |

## <a name="authentication"></a><span data-ttu-id="ebb92-234">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="ebb92-234">Authentication</span></span>

<span data-ttu-id="ebb92-235">Для получения необходимых данных этот контроль [](../providers/providers.md) использует глобального поставщика проверки подлинности, описанного в документации по проверке подлинности.</span><span class="sxs-lookup"><span data-stu-id="ebb92-235">The control uses the global authentication provider described in the [authentication documentation](../providers/providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="ebb92-236">Расширение для большего контроля</span><span class="sxs-lookup"><span data-stu-id="ebb92-236">Extend for more control</span></span>

<span data-ttu-id="ebb92-237">Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов для переопределения `protected render*` в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="ebb92-237">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="ebb92-238">Метод</span><span class="sxs-lookup"><span data-stu-id="ebb92-238">Method</span></span> | <span data-ttu-id="ebb92-239">Описание</span><span class="sxs-lookup"><span data-stu-id="ebb92-239">Description</span></span> |
| - | - |
| <span data-ttu-id="ebb92-240">renderLoading</span><span class="sxs-lookup"><span data-stu-id="ebb92-240">renderLoading</span></span> | <span data-ttu-id="ebb92-241">Отрисовка состояния загрузки.</span><span class="sxs-lookup"><span data-stu-id="ebb92-241">Renders the loading state.</span></span> |
| <span data-ttu-id="ebb92-242">renderNoData</span><span class="sxs-lookup"><span data-stu-id="ebb92-242">renderNoData</span></span> | <span data-ttu-id="ebb92-243">Отрисовка, когда данные изображения или человека недоступны.</span><span class="sxs-lookup"><span data-stu-id="ebb92-243">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="ebb92-244">renderAvatar</span><span class="sxs-lookup"><span data-stu-id="ebb92-244">renderAvatar</span></span> | <span data-ttu-id="ebb92-245">Отрисовка аватара.</span><span class="sxs-lookup"><span data-stu-id="ebb92-245">Renders the avatar.</span></span> |
| <span data-ttu-id="ebb92-246">renderDetails</span><span class="sxs-lookup"><span data-stu-id="ebb92-246">renderDetails</span></span> | <span data-ttu-id="ebb92-247">Отрисовка части сведений о человеке.</span><span class="sxs-lookup"><span data-stu-id="ebb92-247">Renders the person details part.</span></span> |
