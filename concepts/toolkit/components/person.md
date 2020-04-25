---
title: Компонент Person в наборе инструментов Microsoft Graph
description: Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: a23d5432c868881f05c04b84626962d684f7d1eb
ms.sourcegitcommit: d2536f56e3a424219660bc0495ec8632932b4fb8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/25/2020
ms.locfileid: "43812550"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d188a-103">Компонент Person в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d188a-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d188a-104">Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d188a-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span>

<span data-ttu-id="d188a-105">Кроме того, для отображения всплывающей карточки с дополнительными сведениями о пользователе в компоненте Person используется [карточка упр](./person-card.md) ./Person.</span><span class="sxs-lookup"><span data-stu-id="d188a-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="d188a-106">Дополнительные сведения можно найти в разделе [карточка пользователя](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="d188a-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="d188a-107">Пример</span><span class="sxs-lookup"><span data-stu-id="d188a-107">Example</span></span>

<span data-ttu-id="d188a-108">В приведенном ниже примере отображается пользователь, `mgt-person` использующий компонент.</span><span class="sxs-lookup"><span data-stu-id="d188a-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="d188a-109">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="d188a-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="d188a-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="d188a-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="d188a-111">Настройка сведений о лице</span><span class="sxs-lookup"><span data-stu-id="d188a-111">Setting the person details</span></span>

<span data-ttu-id="d188a-112">Для задания сведений о лице можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="d188a-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="d188a-113">Используйте только одно из следующих свойств для каждого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="d188a-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="d188a-114">Задайте `user-id` атрибут или `userId` свойство, чтобы получить пользователя из Microsoft Graph с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="d188a-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="d188a-115">Задайте `person-query` атрибут или `personQuery` свойство для поиска определенного пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d188a-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="d188a-116">Он выбирает первого пользователя, который будет доступен, и извлекает сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="d188a-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="d188a-117">Электронная почта обеспечивает наилучшее обращение к нужному человеку, но имя также работает.</span><span class="sxs-lookup"><span data-stu-id="d188a-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="d188a-118">Задайте `person-details` атрибут или `personDetails` свойство, чтобы вручную задать сведения о лице, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="d188a-118">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        personImage: 'url'
    }
    ```

  <span data-ttu-id="d188a-119">Если изображение не указано, выбирается один из них (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="d188a-119">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="d188a-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="d188a-120">Properties</span></span>

<span data-ttu-id="d188a-121">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="d188a-121">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="d188a-122">Атрибут</span><span class="sxs-lookup"><span data-stu-id="d188a-122">Attribute</span></span>    | <span data-ttu-id="d188a-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="d188a-123">Property</span></span>   | <span data-ttu-id="d188a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d188a-124">Description</span></span>                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| <span data-ttu-id="d188a-125">Show (имя)</span><span class="sxs-lookup"><span data-stu-id="d188a-125">show-name</span></span>    | <span data-ttu-id="d188a-126">шовнаме</span><span class="sxs-lookup"><span data-stu-id="d188a-126">showName</span></span>   | <span data-ttu-id="d188a-127">Установите флаг для отображения отображаемого имени пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="d188a-127">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="d188a-128">Show — email</span><span class="sxs-lookup"><span data-stu-id="d188a-128">show-email</span></span>   | <span data-ttu-id="d188a-129">шовемаил</span><span class="sxs-lookup"><span data-stu-id="d188a-129">showEmail</span></span>  | <span data-ttu-id="d188a-130">Установите флаг для отображения электронной почты пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="d188a-130">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="d188a-131">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="d188a-131">CSS custom properties</span></span>

<span data-ttu-id="d188a-132">`mgt-person` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="d188a-132">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="d188a-133">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="d188a-133">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="d188a-134">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="d188a-134">Templates</span></span>

<span data-ttu-id="d188a-135">`mgt-person` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="d188a-135">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="d188a-136">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="d188a-136">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="d188a-137">Тип данных</span><span class="sxs-lookup"><span data-stu-id="d188a-137">Data type</span></span> | <span data-ttu-id="d188a-138">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="d188a-138">Data context</span></span> | <span data-ttu-id="d188a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="d188a-139">Description</span></span> |
| --------- | ------------ | ----------- |
| <span data-ttu-id="d188a-140">загрузки</span><span class="sxs-lookup"><span data-stu-id="d188a-140">loading</span></span> | <span data-ttu-id="d188a-141">Нет</span><span class="sxs-lookup"><span data-stu-id="d188a-141">none</span></span> | <span data-ttu-id="d188a-142">Шаблон, который будет отображаться, пока компонент находится в состоянии лаодинг.</span><span class="sxs-lookup"><span data-stu-id="d188a-142">The template to render while the component is in a laoding state.</span></span> |
| <span data-ttu-id="d188a-143">нет данных</span><span class="sxs-lookup"><span data-stu-id="d188a-143">no-data</span></span> | <span data-ttu-id="d188a-144">Нет</span><span class="sxs-lookup"><span data-stu-id="d188a-144">none</span></span> | <span data-ttu-id="d188a-145">Шаблон для отображения при отсутствии изображения или данных, доступных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d188a-145">The template to render when no person image or data is available.</span></span> | 
| <span data-ttu-id="d188a-146">умолчани</span><span class="sxs-lookup"><span data-stu-id="d188a-146">default</span></span> | <span data-ttu-id="d188a-147">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="d188a-147">person: The person details object</span></span> <br> <span data-ttu-id="d188a-148">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="d188a-148">`personImage`: The URL of the image</span></span> | <span data-ttu-id="d188a-149">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="d188a-149">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="d188a-150">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="d188a-150">person-card</span></span> | <span data-ttu-id="d188a-151">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="d188a-151">person: The person details object</span></span> <br> <span data-ttu-id="d188a-152">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="d188a-152">`personImage`: The URL of the image</span></span> | <span data-ttu-id="d188a-153">Шаблон для обновления карточки упр. Person, отображаемой при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="d188a-153">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="d188a-154">В следующем примере определяется шаблон для компонента Person.</span><span class="sxs-lookup"><span data-stu-id="d188a-154">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="d188a-155">Карточка пользователя</span><span class="sxs-lookup"><span data-stu-id="d188a-155">Person Card</span></span>

<span data-ttu-id="d188a-156">`mgt-person` Компонент может отображать элемент `mgt-person-card` при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="d188a-156">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="d188a-157">Добавление элемента управления на HTML-страницу</span><span class="sxs-lookup"><span data-stu-id="d188a-157">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="d188a-158">Атрибут</span><span class="sxs-lookup"><span data-stu-id="d188a-158">Attribute</span></span>    |  <span data-ttu-id="d188a-159">Свойство</span><span class="sxs-lookup"><span data-stu-id="d188a-159">Property</span></span>     | <span data-ttu-id="d188a-160">Описание</span><span class="sxs-lookup"><span data-stu-id="d188a-160">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="d188a-161">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="d188a-161">person-card</span></span> | <span data-ttu-id="d188a-162">персонкардинтерактион</span><span class="sxs-lookup"><span data-stu-id="d188a-162">personCardInteraction</span></span> | <span data-ttu-id="d188a-163">Перечисление для определения действия пользователя, необходимого для активации `hover` всплывающей `click`панели.</span><span class="sxs-lookup"><span data-stu-id="d188a-163">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="d188a-164">Значение по умолчанию:`none`</span><span class="sxs-lookup"><span data-stu-id="d188a-164">Default value is `none`</span></span> |


<span data-ttu-id="d188a-165">Для получения дополнительных сведений о шаблонах, стилях и атрибутах обратитесь к [компоненту карточки сотрудника](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="d188a-165">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d188a-166">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d188a-166">Microsoft Graph permissions</span></span>

<span data-ttu-id="d188a-167">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d188a-167">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="d188a-168">Resource</span><span class="sxs-lookup"><span data-stu-id="d188a-168">Resource</span></span>                                                                                                    | <span data-ttu-id="d188a-169">Разрешение</span><span class="sxs-lookup"><span data-stu-id="d188a-169">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="d188a-170">/ме</span><span class="sxs-lookup"><span data-stu-id="d188a-170">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="d188a-171">User.Read</span><span class="sxs-lookup"><span data-stu-id="d188a-171">User.Read</span></span>          |
| [<span data-ttu-id="d188a-172">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="d188a-172">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="d188a-173">User.Read</span><span class="sxs-lookup"><span data-stu-id="d188a-173">User.Read</span></span>          |
| [<span data-ttu-id="d188a-174">/ме/Пеопле/? $search =</span><span class="sxs-lookup"><span data-stu-id="d188a-174">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="d188a-175">People.Read</span><span class="sxs-lookup"><span data-stu-id="d188a-175">People.Read</span></span>        |
| [<span data-ttu-id="d188a-176">/ме/контактс/\*</span><span class="sxs-lookup"><span data-stu-id="d188a-176">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="d188a-177">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d188a-177">Contacts.Read</span></span>      |
| [<span data-ttu-id="d188a-178">/усерс/{ИД}/фото/$value</span><span class="sxs-lookup"><span data-stu-id="d188a-178">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="d188a-179">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d188a-179">User.ReadBasic.All</span></span> |

> <span data-ttu-id="d188a-180">**Примечание:** чтобы получить доступ `*/photo/$value` к ресурсам для личных учетных записей Майкрософт, используйте конечную точку бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d188a-180">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="d188a-181">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="d188a-181">Authentication</span></span>

<span data-ttu-id="d188a-182">Для извлечения необходимых данных элемент управления использует глобальную проверку подлинности, описанную в [документации по проверке подлинности](./../providers.md) .</span><span class="sxs-lookup"><span data-stu-id="d188a-182">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="d188a-183">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="d188a-183">Extend for more control</span></span>

<span data-ttu-id="d188a-184">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет `protected render*` несколько способов переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="d188a-184">For more complex scenarios or a truly custom UX, this component exposes several `protected render*` methods for override in component extensions.</span></span>

| <span data-ttu-id="d188a-185">Метод</span><span class="sxs-lookup"><span data-stu-id="d188a-185">Method</span></span> | <span data-ttu-id="d188a-186">Описание</span><span class="sxs-lookup"><span data-stu-id="d188a-186">Description</span></span> |
| - | - |
| <span data-ttu-id="d188a-187">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="d188a-187">renderLoading</span></span> | <span data-ttu-id="d188a-188">Отображает состояние загрузки.</span><span class="sxs-lookup"><span data-stu-id="d188a-188">Renders the loading state.</span></span> |
| <span data-ttu-id="d188a-189">рендеримаже</span><span class="sxs-lookup"><span data-stu-id="d188a-189">renderImage</span></span> | <span data-ttu-id="d188a-190">Отрисовывает часть изображения.</span><span class="sxs-lookup"><span data-stu-id="d188a-190">Renders the image part.</span></span> |
| <span data-ttu-id="d188a-191">рендернодата</span><span class="sxs-lookup"><span data-stu-id="d188a-191">renderNoData</span></span> | <span data-ttu-id="d188a-192">Отрисовывает, когда нет доступных изображений или данных о пользователях.</span><span class="sxs-lookup"><span data-stu-id="d188a-192">Renders when no image or person data is available.</span></span> |
| <span data-ttu-id="d188a-193">рендердетаилс</span><span class="sxs-lookup"><span data-stu-id="d188a-193">renderDetails</span></span> | <span data-ttu-id="d188a-194">Отрисовывает часть сведений о лице.</span><span class="sxs-lookup"><span data-stu-id="d188a-194">Renders the person details part.</span></span> |
| <span data-ttu-id="d188a-195">рендеремаил</span><span class="sxs-lookup"><span data-stu-id="d188a-195">renderEmail</span></span> | <span data-ttu-id="d188a-196">Отрисовывает часть сведений о лице, вложенную в сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d188a-196">Renders the email sub-part of the person details.</span></span> |
| <span data-ttu-id="d188a-197">рендернаме</span><span class="sxs-lookup"><span data-stu-id="d188a-197">renderName</span></span> | <span data-ttu-id="d188a-198">Отображает имя вложенной части сведений о лице.</span><span class="sxs-lookup"><span data-stu-id="d188a-198">Renders the name sub-part of the person details.</span></span> |
