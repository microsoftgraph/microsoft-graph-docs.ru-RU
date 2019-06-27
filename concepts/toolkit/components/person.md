---
title: Компонент Person в наборе инструментов Microsoft Graph
description: Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9102259258bb691dee2c56449257740db7b1913
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243066"
---
# <a name="person-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="9f133-103">Компонент Person в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9f133-103">Person component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="9f133-104">Компонент Person используется для отображения человека или контакта, используя фотографию, имя и/или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="9f133-104">The person component is used to display a person or contact by using their photo, name, and/or email address.</span></span> 

## <a name="example"></a><span data-ttu-id="9f133-105">Пример</span><span class="sxs-lookup"><span data-stu-id="9f133-105">Example</span></span>

[<span data-ttu-id="9f133-106">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="9f133-106">jsfiddle example</span></span>](https://jsfiddle.net/metulev/0jkzfr42/)

### <a name="add-the-control-to-the-html-page"></a><span data-ttu-id="9f133-107">Добавление элемента управления на HTML-страницу</span><span class="sxs-lookup"><span data-stu-id="9f133-107">Add the control to the HTML page</span></span>
```html
<mgt-person person-query=""></mgt-person>
```

## <a name="setting-the-person-details"></a><span data-ttu-id="9f133-108">Настройка сведений о лице</span><span class="sxs-lookup"><span data-stu-id="9f133-108">Setting the person details</span></span>

<span data-ttu-id="9f133-109">Для задания сведений о лице можно использовать три свойства.</span><span class="sxs-lookup"><span data-stu-id="9f133-109">You can use three properties to set the person details.</span></span> <span data-ttu-id="9f133-110">Используйте только одно из следующих свойств для каждого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="9f133-110">Use only one of the following properties per instance:</span></span>

* <span data-ttu-id="9f133-111">Задайте `user-id` атрибут или `userId` свойство, чтобы получить пользователя из Microsoft Graph с помощью идентификатора.</span><span class="sxs-lookup"><span data-stu-id="9f133-111">Set the `user-id` attribute or `userId` property to fetch the user from Microsoft Graph by using their ID.</span></span>  

* <span data-ttu-id="9f133-112">Задайте `person-query` атрибут или `personQuery` свойство для поиска определенного пользователя в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f133-112">Set the `person-query` attribute or `personQuery` property to search Microsoft Graph for a given person.</span></span> <span data-ttu-id="9f133-113">Он выбирает первого пользователя, который будет доступен, и извлекает сведения о лице.</span><span class="sxs-lookup"><span data-stu-id="9f133-113">It will choose the first person available and fetch the person details.</span></span> <span data-ttu-id="9f133-114">Электронная почта обеспечивает наилучшее обращение к нужному человеку, но имя также работает.</span><span class="sxs-lookup"><span data-stu-id="9f133-114">An email works best to ensure the right person is queried, but a name works as well.</span></span>

* <span data-ttu-id="9f133-115">Задайте `person-details` атрибут или `personDetails` свойство, чтобы вручную задать сведения о лице, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="9f133-115">Set the `person-details` attribute or `personDetails` property to manually set the person details, as shown in the following example.</span></span>


    ```js
    let personControl = document.getElementById('myPersonControl');
    personControl.personDetails = {
        displayName: 'Nikola Metulev',
        email: 'nikola@contoso.com',
        image: 'url'
    }
    ```

  <span data-ttu-id="9f133-116">Если изображение не указано, выбирается один из них (если он доступен).</span><span class="sxs-lookup"><span data-stu-id="9f133-116">If no image is provided, one will be fetched (if available).</span></span>

## <a name="changing-how-the-component-looks"></a><span data-ttu-id="9f133-117">Изменение вида компонента</span><span class="sxs-lookup"><span data-stu-id="9f133-117">Changing how the component looks</span></span>

<span data-ttu-id="9f133-118">Вы можете использовать несколько пропертиесто, чтобы настроить компонент.</span><span class="sxs-lookup"><span data-stu-id="9f133-118">You can use several propertiesto customize the component.</span></span>

| <span data-ttu-id="9f133-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f133-119">Property</span></span> | <span data-ttu-id="9f133-120">Атрибут</span><span class="sxs-lookup"><span data-stu-id="9f133-120">Attribute</span></span> | <span data-ttu-id="9f133-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9f133-121">Description</span></span> |
| --- | --- | --- |
| `showName` | `show-name` | <span data-ttu-id="9f133-122">Установите флаг для отображения отображаемого имени пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="9f133-122">Set flag to display person display name - default is `false`.</span></span> |
| `showEmail` | `show-email` | <span data-ttu-id="9f133-123">Установите флаг для отображения электронной почты пользователя — значение `false`по умолчанию —.</span><span class="sxs-lookup"><span data-stu-id="9f133-123">Set flag to display person email - default is `false`.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="9f133-124">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="9f133-124">CSS custom properties</span></span>

<span data-ttu-id="9f133-125">`mgt-person` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="9f133-125">The `mgt-person` component defines the following CSS custom properties.</span></span>

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

<span data-ttu-id="9f133-126">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="9f133-126">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="9f133-127">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="9f133-127">Templates</span></span>

<span data-ttu-id="9f133-128">`mgt-person` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="9f133-128">The `mgt-person` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="9f133-129">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="9f133-129">To specify a template, include a `<template>` element inside a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="9f133-130">Тип данных</span><span class="sxs-lookup"><span data-stu-id="9f133-130">Data type</span></span> | <span data-ttu-id="9f133-131">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="9f133-131">Data context</span></span> | <span data-ttu-id="9f133-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f133-132">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="9f133-133">`person`: объект Person</span><span class="sxs-lookup"><span data-stu-id="9f133-133">`person`: a person object</span></span> | <span data-ttu-id="9f133-134">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="9f133-134">The default template replaces the entire component with your own.</span></span> |

<span data-ttu-id="9f133-135">В следующем примере определяется шаблон для компонента Person:</span><span class="sxs-lookup"><span data-stu-id="9f133-135">The following example defines a template for the person component:</span></span>

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

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="9f133-136">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9f133-136">Microsoft Graph permissions</span></span>

<span data-ttu-id="9f133-137">Этот элемент управления использует указанные ниже API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f133-137">This control uses the following Microsoft Graph APIs and permissions.</span></span>

| <span data-ttu-id="9f133-138">Ресурс</span><span class="sxs-lookup"><span data-stu-id="9f133-138">Resource</span></span> | <span data-ttu-id="9f133-139">Разрешение или область</span><span class="sxs-lookup"><span data-stu-id="9f133-139">Permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="9f133-140">/ме</span><span class="sxs-lookup"><span data-stu-id="9f133-140">/me</span></span>](https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0) | `User.Read` |
| [<span data-ttu-id="9f133-141">/ме/фото/$value</span><span class="sxs-lookup"><span data-stu-id="9f133-141">/me/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/profilephoto-get?view=graph-rest-beta) | `User.Read` |
| [<span data-ttu-id="9f133-142">/ме/Пеопле/? $search =</span><span class="sxs-lookup"><span data-stu-id="9f133-142">/me/people/?$search=</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `People.Read` |
| [<span data-ttu-id="9f133-143">/ме/контактс/\*</span><span class="sxs-lookup"><span data-stu-id="9f133-143">/me/contacts/\*</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=cs) | `Contacts.Read` |
| [<span data-ttu-id="9f133-144">/усерс/{ИД}/фото/$value</span><span class="sxs-lookup"><span data-stu-id="9f133-144">/users/{id}/photo/$value</span></span>](https://docs.microsoft.com/en-us/graph/api/user-list-people?view=graph-rest-1.0) | `User.ReadBasic.All` |

> <span data-ttu-id="9f133-145">**Примечание:** чтобы получить доступ `*/photo/$value` к ресурсам для личных учетных записей Майкрософт, используйте конечную точку бета-версии Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="9f133-145">**Note:** to access the `*/photo/$value` resources for personal Microsoft accounts, use the Microsoft Graph beta endpoint.</span></span>

## <a name="authentication"></a><span data-ttu-id="9f133-146">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="9f133-146">Authentication</span></span>

<span data-ttu-id="9f133-147">Для извлечения необходимых данных элемент управления использует глобальную проверку подлинности, описанную в [документации по проверке](./../providers.md) подлинности.</span><span class="sxs-lookup"><span data-stu-id="9f133-147">The control uses the global authentication provider described in the [authentication documentation](./../providers.md) to fetch the required data.</span></span>
