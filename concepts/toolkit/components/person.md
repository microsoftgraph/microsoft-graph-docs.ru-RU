---
title: Компонент Person в наборе инструментов Microsoft Graph
description: Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: ab9dc1bef81585bb71cdb29de015d8adb6030110
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955857"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="d7de4-103">Компонент Person в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d7de4-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="d7de4-104">Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d7de4-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span> 

<span data-ttu-id="d7de4-105">Кроме того, для отображения всплывающей карточки с дополнительными сведениями о пользователе в компоненте Person используется [карточка упр](./person-card.md) ./Person.</span><span class="sxs-lookup"><span data-stu-id="d7de4-105">The person component also uses the [mgt-person-card](./person-card.md) to display a flyout card with additional information about the user.</span></span> <span data-ttu-id="d7de4-106">Дополнительные сведения можно найти в разделе [карточка пользователя](#person-card) .</span><span class="sxs-lookup"><span data-stu-id="d7de4-106">For details, see the [Person Card](#person-card) section.</span></span>

## <a name="example"></a><span data-ttu-id="d7de4-107">Пример</span><span class="sxs-lookup"><span data-stu-id="d7de4-107">Example</span></span>

[<span data-ttu-id="d7de4-108">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="d7de4-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="d7de4-109">Добавление элемента управления на HTML-страницу</span><span class="sxs-lookup"><span data-stu-id="d7de4-109">Add the control to the HTML page</span></span>
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a><span data-ttu-id="d7de4-110">Настройка сведений о лице</span><span class="sxs-lookup"><span data-stu-id="d7de4-110">Setting the person details</span></span>

<span data-ttu-id="d7de4-111">Для задания сведений о лице можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="d7de4-111">You can use three properties to set the person details.</span></span> <span data-ttu-id="d7de4-112">Используйте только одно из следующих свойств для каждого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="d7de4-112">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="d7de4-113">Задайте `user-id` атрибут или `userId` свойство, чтобы получить пользователя из Microsoft Graph с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="d7de4-113">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>  

* <span data-ttu-id="d7de4-114">Задайте `person-query` атрибут или `personQuery` свойство для поиска определенного пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d7de4-114">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="d7de4-115">Он выбирает первого пользователя, который будет доступен, и извлекает сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="d7de4-115">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="d7de4-116">Электронная почта обеспечивает наилучшее обращение к нужному человеку, но имя также работает.</span><span class="sxs-lookup"><span data-stu-id="d7de4-116">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="d7de4-117">Задайте `person-details` атрибут или `personDetails` свойство, чтобы вручную задать сведения о лице, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="d7de4-117">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="d7de4-118">Если изображение не указано, выбирается один из них (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="d7de4-118">If no image is provided, one will be fetched (if available).</span></span>

## <a name="changing-how-the-component-looks"></a><span data-ttu-id="d7de4-119">Изменение вида компонента</span><span class="sxs-lookup"><span data-stu-id="d7de4-119">Changing how the component looks</span></span>

<span data-ttu-id="d7de4-120">Для настройки компонента можно использовать несколько свойств.</span><span class="sxs-lookup"><span data-stu-id="d7de4-120">You can use several properties to customize the component.</span></span>

| <span data-ttu-id="d7de4-121">Атрибут</span><span class="sxs-lookup"><span data-stu-id="d7de4-121">Attribute</span></span>    | <span data-ttu-id="d7de4-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7de4-122">Property</span></span>   | <span data-ttu-id="d7de4-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d7de4-123">Description</span></span>                                                   |
| -----------  | ---------- | ------------------------------------------------------------- |
| <span data-ttu-id="d7de4-124">Show (имя)</span><span class="sxs-lookup"><span data-stu-id="d7de4-124">show-name</span></span>    | <span data-ttu-id="d7de4-125">шовнаме</span><span class="sxs-lookup"><span data-stu-id="d7de4-125">showName</span></span>   | <span data-ttu-id="d7de4-126">Установите флаг для отображения отображаемого имени пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="d7de4-126">Set flag to display person display name - default is `false`.</span></span> |
| <span data-ttu-id="d7de4-127">Show — email</span><span class="sxs-lookup"><span data-stu-id="d7de4-127">show-email</span></span>   | <span data-ttu-id="d7de4-128">шовемаил</span><span class="sxs-lookup"><span data-stu-id="d7de4-128">showEmail</span></span>  | <span data-ttu-id="d7de4-129">Установите флаг для отображения электронной почты пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="d7de4-129">Set flag to display person email - default is `false`.</span></span>        |

## <a name="css-custom-properties"></a><span data-ttu-id="d7de4-130">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="d7de4-130">CSS custom properties</span></span>

<span data-ttu-id="d7de4-131">`mgt-person` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="d7de4-131">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="d7de4-132">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="d7de4-132">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="d7de4-133">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="d7de4-133">Templates</span></span>

<span data-ttu-id="d7de4-134">`mgt-person` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="d7de4-134">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="d7de4-135">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="d7de4-135">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="d7de4-136">Тип данных</span><span class="sxs-lookup"><span data-stu-id="d7de4-136">Data type</span></span>     | <span data-ttu-id="d7de4-137">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="d7de4-137">Data context</span></span>              | <span data-ttu-id="d7de4-138">Описание</span><span class="sxs-lookup"><span data-stu-id="d7de4-138">Description</span></span>                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| <span data-ttu-id="d7de4-139">умолчани</span><span class="sxs-lookup"><span data-stu-id="d7de4-139">default</span></span>     | <span data-ttu-id="d7de4-140">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="d7de4-140">person: The person details object</span></span> <br> <span data-ttu-id="d7de4-141">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="d7de4-141">`personImage`: The URL of the image</span></span> | <span data-ttu-id="d7de4-142">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="d7de4-142">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="d7de4-143">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="d7de4-143">person-card</span></span> | <span data-ttu-id="d7de4-144">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="d7de4-144">person: The person details object</span></span> <br> <span data-ttu-id="d7de4-145">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="d7de4-145">`personImage`: The URL of the image</span></span> | <span data-ttu-id="d7de4-146">Шаблон для обновления карточки упр. Person, отображаемой при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="d7de4-146">The template to update the mgt-person-card displayed on hover or click.</span></span> |

<span data-ttu-id="d7de4-147">В следующем примере определяется шаблон для компонента Person.</span><span class="sxs-lookup"><span data-stu-id="d7de4-147">The following example defines a template for the person component.</span></span>

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

## <a name="person-card"></a><span data-ttu-id="d7de4-148">Карточка лица</span><span class="sxs-lookup"><span data-stu-id="d7de4-148">Person Card</span></span>

<span data-ttu-id="d7de4-149">`mgt-person` Компонент может отображать элемент `mgt-person-card` при наведении или щелчке мышью.</span><span class="sxs-lookup"><span data-stu-id="d7de4-149">The `mgt-person` component can show an `mgt-person-card` on either hover or click.</span></span>

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="d7de4-150">Добавление элемента управления на HTML-страницу</span><span class="sxs-lookup"><span data-stu-id="d7de4-150">Add the control to the HTML page</span></span>
```html
<mgt-person person-query="me" person-card="hover"></mgt-person>
```

| <span data-ttu-id="d7de4-151">Атрибут</span><span class="sxs-lookup"><span data-stu-id="d7de4-151">Attribute</span></span>    |  <span data-ttu-id="d7de4-152">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7de4-152">Property</span></span>     | <span data-ttu-id="d7de4-153">Описание</span><span class="sxs-lookup"><span data-stu-id="d7de4-153">Description</span></span>                                                                     |
| ------------ | ------------- | ------------------------------------------------------------------------------- |
| <span data-ttu-id="d7de4-154">Person — карточка</span><span class="sxs-lookup"><span data-stu-id="d7de4-154">person-card</span></span> | <span data-ttu-id="d7de4-155">персонкард</span><span class="sxs-lookup"><span data-stu-id="d7de4-155">personCard</span></span> | <span data-ttu-id="d7de4-156">Перечисление для определения действия пользователя, необходимого для активации `hover` всплывающей `click`панели.</span><span class="sxs-lookup"><span data-stu-id="d7de4-156">An enumeration to determine user action necessary to activate flyout panel - `hover` or `click`.</span></span> <span data-ttu-id="d7de4-157">Значение по умолчанию:`none`</span><span class="sxs-lookup"><span data-stu-id="d7de4-157">Default value is `none`</span></span> |


<span data-ttu-id="d7de4-158">Для получения дополнительных сведений о шаблонах, стилях и атрибутах обратитесь к [компоненту карточки сотрудника](./person-card.md).</span><span class="sxs-lookup"><span data-stu-id="d7de4-158">For more information about templating, styling, and attributes, see [Person Card component](./person-card.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="d7de4-159">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d7de4-159">Microsoft Graph permissions</span></span>

<span data-ttu-id="d7de4-160">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d7de4-160">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="d7de4-161">Resource</span><span class="sxs-lookup"><span data-stu-id="d7de4-161">Resource</span></span>                                                                                                    | <span data-ttu-id="d7de4-162">Разрешение</span><span class="sxs-lookup"><span data-stu-id="d7de4-162">Permission</span></span>     |
| ----------------------------------------------------------------------------------------------------------- | -------------------- |
| [<span data-ttu-id="d7de4-163">/ме</span><span class="sxs-lookup"><span data-stu-id="d7de4-163">/me</span></span>](https://docs.microsoft.com/graph/api/user-get?view=graph-rest-1.0)                              | <span data-ttu-id="d7de4-164">User.Read</span><span class="sxs-lookup"><span data-stu-id="d7de4-164">User.Read</span></span>          |
| [<span data-ttu-id="d7de4-165">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="d7de4-165">/me/photo/$value</span></span>](https://docs.microsoft.com/graph/api/profilephoto-get?view=graph-rest-beta)        | <span data-ttu-id="d7de4-166">User.Read</span><span class="sxs-lookup"><span data-stu-id="d7de4-166">User.Read</span></span>          |
| [<span data-ttu-id="d7de4-167">/ме/Пеопле/? $search =</span><span class="sxs-lookup"><span data-stu-id="d7de4-167">/me/people/?$search=</span></span>](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0)     | <span data-ttu-id="d7de4-168">People.Read</span><span class="sxs-lookup"><span data-stu-id="d7de4-168">People.Read</span></span>        |
| [<span data-ttu-id="d7de4-169">/ме/контактс/\*</span><span class="sxs-lookup"><span data-stu-id="d7de4-169">/me/contacts/\*</span></span>](https://docs.microsoft.com/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | <span data-ttu-id="d7de4-170">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="d7de4-170">Contacts.Read</span></span>      |
| [<span data-ttu-id="d7de4-171">/усерс/{ИД}/фото/$value</span><span class="sxs-lookup"><span data-stu-id="d7de4-171">/users/{id}/photo/$value</span></span>](https://docs.microsoft.com/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="d7de4-172">User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="d7de4-172">User.ReadBasic.All</span></span> |

> <span data-ttu-id="d7de4-173">**Примечание:** чтобы получить доступ `*/photo/$value` к ресурсам для личных учетных записей Майкрософт, используйте конечную точку бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d7de4-173">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="d7de4-174">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="d7de4-174">Authentication</span></span>

<span data-ttu-id="d7de4-175">Для извлечения необходимых данных элемент управления использует глобальную проверку подлинности, описанную в [документации по проверке подлинности](./../providers.md) .</span><span class="sxs-lookup"><span data-stu-id="d7de4-175">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
