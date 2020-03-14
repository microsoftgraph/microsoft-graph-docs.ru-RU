---
title: Компонент Person в наборе инструментов Microsoft Graph
description: Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0202d8bc8c8ae23f98cb4add9f9d5ca96afea04d
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639956"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="950fe-103">Компонент Person в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="950fe-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="950fe-104">Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="950fe-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span>

<span data-ttu-id="950fe-105">Кроме того, для отображения всплывающей карточки с дополнительными сведениями о пользователе в компоненте Person используется [карточка упр](./person-card.md) ./Person.</span><span class="sxs-lookup"><span data-stu-id="950fe-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="950fe-106">Дополнительные сведения можно найти в разделе [карточка пользователя](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="950fe-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="950fe-107">Пример</span><span class="sxs-lookup"><span data-stu-id="950fe-107">Example</span></span>

<span data-ttu-id="950fe-108">В приведенном ниже примере отображается пользователь, `mgt-person` использующий компонент.</span><span class="sxs-lookup"><span data-stu-id="950fe-108">The following example displays a person using the `mgt-person` component.</span></span> <span data-ttu-id="950fe-109">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="950fe-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person--person&source=docs" height="250"></iframe>

[<span data-ttu-id="950fe-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="950fe-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person--person&source=docs)

## <a name="setting-the-person-details"></a><span data-ttu-id="950fe-111">Настройка сведений о лице</span><span class="sxs-lookup"><span data-stu-id="950fe-111">Setting the person details</span></span>

<span data-ttu-id="950fe-112">Для задания сведений о лице можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="950fe-112">You can use three properties to set the person details.</span></span> <span data-ttu-id="950fe-113">Используйте только одно из следующих свойств для каждого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="950fe-113">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="950fe-114">Задайте `user-id` атрибут или `userId` свойство, чтобы получить пользователя из Microsoft Graph с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="950fe-114">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>

* <span data-ttu-id="950fe-115">Задайте `person-query` атрибут или `personQuery` свойство для поиска определенного пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="950fe-115">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="950fe-116">Он выбирает первого пользователя, который будет доступен, и извлекает сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="950fe-116">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="950fe-117">Электронная почта обеспечивает наилучшее обращение к нужному человеку, но имя также работает.</span><span class="sxs-lookup"><span data-stu-id="950fe-117">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="950fe-118">Задайте `person-details` атрибут или `personDetails` свойство, чтобы вручную задать сведения о лице, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="950fe-118">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="950fe-119">Если изображение не указано, выбирается один из них (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="950fe-119">If no image is provided, one will be fetched (if available).</span></span>

## <a name="properties"></a><span data-ttu-id="950fe-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="950fe-120">Properties</span></span>

<span data-ttu-id="950fe-121">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="950fe-121">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="950fe-122">Атрибут</span><span class="sxs-lookup"><span data-stu-id="950fe-122">Attribute</span></span>    | <span data-ttu-id="950fe-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="950fe-123">Property</span></span>   | <span data-ttu-id="950fe-124">Описание</span><span class="sxs-lookup"><span data-stu-id="950fe-124">Description</span></span>                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| <span data-ttu-id="950fe-125">Show (имя)</span><span class="sxs-lookup"><span data-stu-id="950fe-125">show-name</span></span>    | <span data-ttu-id="950fe-126">шовнаме</span><span class="sxs-lookup"><span data-stu-id="950fe-126">showName</span></span>   | <span data-ttu-id="950fe-127">Установите флаг для отображения отображаемого имени пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="950fe-127">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="950fe-128">Show — email</span><span class="sxs-lookup"><span data-stu-id="950fe-128">show-email</span></span>   | <span data-ttu-id="950fe-129">шовемаил</span><span class="sxs-lookup"><span data-stu-id="950fe-129">showEmail</span></span>  | <span data-ttu-id="950fe-130">Установите флаг для отображения электронной почты пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="950fe-130">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="950fe-131">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="950fe-131">CSS custom properties</span></span>

<span data-ttu-id="950fe-132">`mgt-person` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="950fe-132">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="950fe-133">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="950fe-133">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="950fe-134">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="950fe-134">Templates</span></span>

<span data-ttu-id="950fe-135">`mgt-person` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="950fe-135">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="950fe-136">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="950fe-136">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="950fe-137">Тип данных</span><span class="sxs-lookup"><span data-stu-id="950fe-137">Data type</span></span>     | <span data-ttu-id="950fe-138">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="950fe-138">Data context</span></span>              | <span data-ttu-id="950fe-139">Описание</span><span class="sxs-lookup"><span data-stu-id="950fe-139">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="950fe-140">умолчани</span><span class="sxs-lookup"><span data-stu-id="950fe-140">default</span></span>     | <span data-ttu-id="950fe-141">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="950fe-141">person: The person details object</span></span> <br> <span data-ttu-id="950fe-142">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="950fe-142">`personImage`: The URL of the image</span></span> | <span data-ttu-id="950fe-143">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="950fe-143">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="950fe-144">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="950fe-144">person-card</span></span> | <span data-ttu-id="950fe-145">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="950fe-145">person: The person details object</span></span> <br> <span data-ttu-id="950fe-146">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="950fe-146">`personImage`: The URL of the image</span></span> | <span data-ttu-id="950fe-147">Шаблон для обновления карточки упр. Person, отображаемой при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="950fe-147">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="950fe-148">В следующем примере определяется шаблон для компонента Person.</span><span class="sxs-lookup"><span data-stu-id="950fe-148">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="950fe-149">Карточка физического лица</span><span class="sxs-lookup"><span data-stu-id="950fe-149">Person Card</span></span>

<span data-ttu-id="950fe-150">`mgt-person` Компонент может отображать элемент `mgt-person-card` при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="950fe-150">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="950fe-151">Добавление элемента управления на HTML-страницу</span><span class="sxs-lookup"><span data-stu-id="950fe-151">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="950fe-152">Атрибут</span><span class="sxs-lookup"><span data-stu-id="950fe-152">Attribute</span></span>    |  <span data-ttu-id="950fe-153">Свойство</span><span class="sxs-lookup"><span data-stu-id="950fe-153">Property</span></span>     | <span data-ttu-id="950fe-154">Описание</span><span class="sxs-lookup"><span data-stu-id="950fe-154">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="950fe-155">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="950fe-155">person-card</span></span> | <span data-ttu-id="950fe-156">персонкард</span><span class="sxs-lookup"><span data-stu-id="950fe-156">personCard</span></span> | <span data-ttu-id="950fe-157">Перечисление для определения действия пользователя, необходимого для активации `hover` всплывающей `click`панели.</span><span class="sxs-lookup"><span data-stu-id="950fe-157">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="950fe-158">Значение по умолчанию:`none`</span><span class="sxs-lookup"><span data-stu-id="950fe-158">Default value is `none`</span></span> |


<span data-ttu-id="950fe-159">Для получения дополнительных сведений о шаблонах, стилях и атрибутах обратитесь к [компоненту карточки сотрудника](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="950fe-159">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="950fe-160">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="950fe-160">Microsoft Graph permissions</span></span>

<span data-ttu-id="950fe-161">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="950fe-161">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="950fe-162">Resource</span><span class="sxs-lookup"><span data-stu-id="950fe-162">Resource</span></span>                                                                                                    | <span data-ttu-id="950fe-163">Разрешение</span><span class="sxs-lookup"><span data-stu-id="950fe-163">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="950fe-164">/ме</span><span class="sxs-lookup"><span data-stu-id="950fe-164">/me</span></span>](/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="950fe-165">User.Read</span><span class="sxs-lookup"><span data-stu-id="950fe-165">User.Read</span></span>          |
| [<span data-ttu-id="950fe-166">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="950fe-166">/me/photo/$value</span></span>](/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="950fe-167">User.Read</span><span class="sxs-lookup"><span data-stu-id="950fe-167">User.Read</span></span>          |
| [<span data-ttu-id="950fe-168">/ме/Пеопле/? $search =</span><span class="sxs-lookup"><span data-stu-id="950fe-168">/me/people/?$search=</span></span>](/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="950fe-169">People.Read</span><span class="sxs-lookup"><span data-stu-id="950fe-169">People.Read</span></span>        |
| [<span data-ttu-id="950fe-170">/ме/контактс/\*</span><span class="sxs-lookup"><span data-stu-id="950fe-170">/me/contacts/\*</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="950fe-171">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="950fe-171">Contacts.Read</span></span>      |
| [<span data-ttu-id="950fe-172">/усерс/{ИД}/фото/$value</span><span class="sxs-lookup"><span data-stu-id="950fe-172">/users/{id}/photo/$value</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="950fe-173">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="950fe-173">User.ReadBasic.All</span></span> |

> <span data-ttu-id="950fe-174">**Примечание:** чтобы получить доступ `*/photo/$value` к ресурсам для личных учетных записей Майкрософт, используйте конечную точку бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="950fe-174">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="950fe-175">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="950fe-175">Authentication</span></span>

<span data-ttu-id="950fe-176">Для извлечения необходимых данных элемент управления использует глобальную проверку подлинности, описанную в [документации по проверке подлинности](./../providers.md) .</span><span class="sxs-lookup"><span data-stu-id="950fe-176">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
