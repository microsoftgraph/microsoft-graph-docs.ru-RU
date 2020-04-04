---
title: Компонент Person в наборе инструментов Microsoft Graph
description: Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 53cd4d8bb7a2bb23a3c54924ee07b4843e7fc503
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144284"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="0cd24-103">Компонент Person в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0cd24-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="0cd24-104">Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0cd24-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span>

<span data-ttu-id="0cd24-105">Кроме того, для отображения всплывающей карточки с дополнительными сведениями о пользователе в компоненте Person используется [карточка упр](./person-card.md) ./Person.</span><span class="sxs-lookup"><span data-stu-id="0cd24-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="0cd24-106">Дополнительные сведения можно найти в разделе [карточка пользователя](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="0cd24-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="0cd24-107">Пример</span><span class="sxs-lookup"><span data-stu-id="0cd24-107">Example</span></span>

<span data-ttu-id="0cd24-108">В приведенном ниже примере отображается пользователь, `mgt-person` использующий компонент.</span><span class="sxs-lookup"><span data-stu-id="0cd24-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="0cd24-109">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="0cd24-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="0cd24-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="0cd24-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="0cd24-111">Настройка сведений о лице</span><span class="sxs-lookup"><span data-stu-id="0cd24-111">Setting the person details</span></span>

<span data-ttu-id="0cd24-112">Для задания сведений о лице можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="0cd24-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="0cd24-113">Используйте только одно из следующих свойств для каждого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="0cd24-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="0cd24-114">Задайте `user-id` атрибут или `userId` свойство, чтобы получить пользователя из Microsoft Graph с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="0cd24-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="0cd24-115">Задайте `person-query` атрибут или `personQuery` свойство для поиска определенного пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0cd24-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="0cd24-116">Он выбирает первого пользователя, который будет доступен, и извлекает сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="0cd24-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="0cd24-117">Электронная почта обеспечивает наилучшее обращение к нужному человеку, но имя также работает.</span><span class="sxs-lookup"><span data-stu-id="0cd24-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="0cd24-118">Задайте `person-details` атрибут или `personDetails` свойство, чтобы вручную задать сведения о лице, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="0cd24-118">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="0cd24-119">Если изображение не указано, выбирается один из них (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="0cd24-119">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="0cd24-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="0cd24-120">Properties</span></span>

<span data-ttu-id="0cd24-121">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="0cd24-121">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="0cd24-122">Атрибут</span><span class="sxs-lookup"><span data-stu-id="0cd24-122">Attribute</span></span>    | <span data-ttu-id="0cd24-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cd24-123">Property</span></span>   | <span data-ttu-id="0cd24-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd24-124">Description</span></span>                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| <span data-ttu-id="0cd24-125">Show (имя)</span><span class="sxs-lookup"><span data-stu-id="0cd24-125">show-name</span></span>    | <span data-ttu-id="0cd24-126">шовнаме</span><span class="sxs-lookup"><span data-stu-id="0cd24-126">showName</span></span>   | <span data-ttu-id="0cd24-127">Установите флаг для отображения отображаемого имени пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="0cd24-127">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="0cd24-128">Show — email</span><span class="sxs-lookup"><span data-stu-id="0cd24-128">show-email</span></span>   | <span data-ttu-id="0cd24-129">шовемаил</span><span class="sxs-lookup"><span data-stu-id="0cd24-129">showEmail</span></span>  | <span data-ttu-id="0cd24-130">Установите флаг для отображения электронной почты пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="0cd24-130">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="0cd24-131">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="0cd24-131">CSS custom properties</span></span>

<span data-ttu-id="0cd24-132">`mgt-person` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="0cd24-132">The `mgt-person` component defines the following CSS custom properties.</span></span>

```css
mgt-person {
  --avatar-size-s: 24px;
  --avatar-size: 48px; // avatar size when both name and email are shown
  --avatar-font-size--s: 16px;
  --avatar-font-size: 32px; // font-size when both name and email are shown
  --avatar-border: 0;
  --initials-color: white;
  --initials-background-color: magenta;
  --font-size: 12px;
  --font-weight: 500;
  --color: black;
  --email-font-size: 12px;
  --email-color: black;
}
```

<span data-ttu-id="0cd24-133">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="0cd24-133">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="0cd24-134">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="0cd24-134">Templates</span></span>

<span data-ttu-id="0cd24-135">`mgt-person` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="0cd24-135">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="0cd24-136">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="0cd24-136">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="0cd24-137">Тип данных</span><span class="sxs-lookup"><span data-stu-id="0cd24-137">Data type</span></span> | <span data-ttu-id="0cd24-138">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="0cd24-138">Data context</span></span> | <span data-ttu-id="0cd24-139">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd24-139">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="0cd24-140">загрузки</span><span class="sxs-lookup"><span data-stu-id="0cd24-140">loading</span></span> | <span data-ttu-id="0cd24-141">нет</span><span class="sxs-lookup"><span data-stu-id="0cd24-141">none</span></span> | <span data-ttu-id="0cd24-142">Шаблон, который будет отображаться, пока компонент находится в состоянии лаодинг.</span><span class="sxs-lookup"><span data-stu-id="0cd24-142">The template to render while the component is in a laoding state.</span></span> |
| <span data-ttu-id="0cd24-143">нет данных</span><span class="sxs-lookup"><span data-stu-id="0cd24-143">no-data</span></span> | <span data-ttu-id="0cd24-144">нет</span><span class="sxs-lookup"><span data-stu-id="0cd24-144">none</span></span> | <span data-ttu-id="0cd24-145">Шаблон для отображения при отсутствии изображения или данных, доступных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="0cd24-145">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="0cd24-146">умолчани</span><span class="sxs-lookup"><span data-stu-id="0cd24-146">default</span></span> | <span data-ttu-id="0cd24-147">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="0cd24-147">person: The person details object</span></span> <br> <span data-ttu-id="0cd24-148">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="0cd24-148">`personImage`: The URL of the image</span></span> | <span data-ttu-id="0cd24-149">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="0cd24-149">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="0cd24-150">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="0cd24-150">person-card</span></span> | <span data-ttu-id="0cd24-151">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="0cd24-151">person: The person details object</span></span> <br> <span data-ttu-id="0cd24-152">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="0cd24-152">`personImage`: The URL of the image</span></span> | <span data-ttu-id="0cd24-153">Шаблон для обновления карточки упр. Person, отображаемой при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="0cd24-153">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="0cd24-154">В следующем примере определяется шаблон для компонента Person.</span><span class="sxs-lookup"><span data-stu-id="0cd24-154">The following example defines a template for the person component.</span></span>

```html
<mgt-person>
  <template>
    <div data-if="person.image">
      <img src="{{person.image}}" />
    </div>
    <div data-else>
      {{person.displayName}}
    </div>
  </template>
</mgt-person>
```

## <a name="person-card"></a><span data-ttu-id="0cd24-155">Карточка физического лица</span><span class="sxs-lookup"><span data-stu-id="0cd24-155">Person Card</span></span>

<span data-ttu-id="0cd24-156">`mgt-person` Компонент может отображать элемент `mgt-person-card` при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="0cd24-156">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="0cd24-157">Добавление элемента управления на HTML-страницу</span><span class="sxs-lookup"><span data-stu-id="0cd24-157">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="0cd24-158">Атрибут</span><span class="sxs-lookup"><span data-stu-id="0cd24-158">Attribute</span></span>    |  <span data-ttu-id="0cd24-159">Свойство</span><span class="sxs-lookup"><span data-stu-id="0cd24-159">Property</span></span>     | <span data-ttu-id="0cd24-160">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd24-160">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="0cd24-161">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="0cd24-161">person-card</span></span> | <span data-ttu-id="0cd24-162">персонкардинтерактион</span><span class="sxs-lookup"><span data-stu-id="0cd24-162">personCardInteraction</span></span> | <span data-ttu-id="0cd24-163">Перечисление для определения действия пользователя, необходимого для активации `hover` всплывающей `click`панели.</span><span class="sxs-lookup"><span data-stu-id="0cd24-163">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="0cd24-164">Значение по умолчанию:`none`</span><span class="sxs-lookup"><span data-stu-id="0cd24-164">Default value is `none`</span></span> |


<span data-ttu-id="0cd24-165">Для получения дополнительных сведений о шаблонах, стилях и атрибутах обратитесь к [компоненту карточки сотрудника](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="0cd24-165">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="0cd24-166">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0cd24-166">Microsoft Graph permissions</span></span>

<span data-ttu-id="0cd24-167">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0cd24-167">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="0cd24-168">Ресурс</span><span class="sxs-lookup"><span data-stu-id="0cd24-168">Resource</span></span>                                                                                                    | <span data-ttu-id="0cd24-169">Разрешение</span><span class="sxs-lookup"><span data-stu-id="0cd24-169">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="0cd24-170">/ме</span><span class="sxs-lookup"><span data-stu-id="0cd24-170">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="0cd24-171">User.Read</span><span class="sxs-lookup"><span data-stu-id="0cd24-171">User.Read</span></span>          |
| [<span data-ttu-id="0cd24-172">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="0cd24-172">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="0cd24-173">User.Read</span><span class="sxs-lookup"><span data-stu-id="0cd24-173">User.Read</span></span>          |
| [<span data-ttu-id="0cd24-174">/ме/Пеопле/? $search =</span><span class="sxs-lookup"><span data-stu-id="0cd24-174">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="0cd24-175">People.Read</span><span class="sxs-lookup"><span data-stu-id="0cd24-175">People.Read</span></span>        |
| [<span data-ttu-id="0cd24-176">/ме/контактс/\*</span><span class="sxs-lookup"><span data-stu-id="0cd24-176">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="0cd24-177">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="0cd24-177">Contacts.Read</span></span>      |
| [<span data-ttu-id="0cd24-178">/усерс/{ИД}/фото/$value</span><span class="sxs-lookup"><span data-stu-id="0cd24-178">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="0cd24-179">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="0cd24-179">User.ReadBasic.All</span></span> |

> <span data-ttu-id="0cd24-180">**Примечание:** чтобы получить доступ `*/photo/$value` к ресурсам для личных учетных записей Майкрософт, используйте конечную точку бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0cd24-180">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="0cd24-181">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="0cd24-181">Authentication</span></span>

<span data-ttu-id="0cd24-182">Для извлечения необходимых данных элемент управления использует глобальную проверку подлинности, описанную в [документации по проверке подлинности](./../providers.md) .</span><span class="sxs-lookup"><span data-stu-id="0cd24-182">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="0cd24-183">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="0cd24-183">Extend for more control</span></span>

<span data-ttu-id="0cd24-184">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет `protected render*` несколько способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="0cd24-184">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="0cd24-185">Метод</span><span class="sxs-lookup"><span data-stu-id="0cd24-185">Method</span></span> | <span data-ttu-id="0cd24-186">Описание</span><span class="sxs-lookup"><span data-stu-id="0cd24-186">Description</span></span> |
| - | - |
| <span data-ttu-id="0cd24-187">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="0cd24-187">renderLoading</span></span> | <span data-ttu-id="0cd24-188">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="0cd24-188">Renders the loading state.</span></span> |
| <span data-ttu-id="0cd24-189">рендеримаже</span><span class="sxs-lookup"><span data-stu-id="0cd24-189">renderImage</span></span> | <span data-ttu-id="0cd24-190">Отрисовывает часть изображения.</span><span class="sxs-lookup"><span data-stu-id="0cd24-190">Renders the image part.</span></span> |
| <span data-ttu-id="0cd24-191">рендернодата</span><span class="sxs-lookup"><span data-stu-id="0cd24-191">renderNoData</span></span> | <span data-ttu-id="0cd24-192">Отрисовывает, когда нет доступных изображений или данных о пользователях.</span><span class="sxs-lookup"><span data-stu-id="0cd24-192">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="0cd24-193">рендердетаилс</span><span class="sxs-lookup"><span data-stu-id="0cd24-193">renderDetails</span></span> | <span data-ttu-id="0cd24-194">Отрисовывает часть сведений о лице.</span><span class="sxs-lookup"><span data-stu-id="0cd24-194">Renders the person details part.</span></span> |
| <span data-ttu-id="0cd24-195">рендеремаил</span><span class="sxs-lookup"><span data-stu-id="0cd24-195">renderEmail</span></span> | <span data-ttu-id="0cd24-196">Отрисовывает часть сведений о лице, вложенную в сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="0cd24-196">Renders the email sub-part of the person details.</span></span> |
| <span data-ttu-id="0cd24-197">рендернаме</span><span class="sxs-lookup"><span data-stu-id="0cd24-197">renderName</span></span> | <span data-ttu-id="0cd24-198">Отображает имя вложенной части сведений о лице.</span><span class="sxs-lookup"><span data-stu-id="0cd24-198">Renders the name sub-part of the person details.</span></span> |
