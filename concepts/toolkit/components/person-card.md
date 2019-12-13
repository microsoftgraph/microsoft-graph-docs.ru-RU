---
title: Компонент Person Card в наборе инструментов Microsoft Graph
description: Компонент Person-Card является компонентом для отображения дополнительных сведений, относящихся к пользователю.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 7f4f20773b152db037d3b57481aa5e8638866f52
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39955871"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="92b29-103">Компонент Person Card в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92b29-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="92b29-104">Компонент Person-Card — это реагирующий на работу компонент для отображения дополнительных сведений, относящихся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="92b29-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="92b29-105">Он обычно используется в качестве всплывающего элемента в `mgt-person` компоненте.</span><span class="sxs-lookup"><span data-stu-id="92b29-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="92b29-106">Дополнительную информацию о компоненте `mgt-person` можно узнать в статье [упр](./person.md).</span><span class="sxs-lookup"><span data-stu-id="92b29-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>
  
## <a name="example"></a><span data-ttu-id="92b29-107">Пример</span><span class="sxs-lookup"><span data-stu-id="92b29-107">Example</span></span>

```html
<mgt-person-card person-details="{personObject}" person-image="imgUrl"></mgt-person-card>
```

## <a name="properties"></a><span data-ttu-id="92b29-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="92b29-108">Properties</span></span>

<span data-ttu-id="92b29-109">Компонент использует Microsoft Graph для предоставления дополнительных сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="92b29-109">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="92b29-110">Чтобы определить пользователя, необходимо использовать свойство **Person — запрос** `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="92b29-110">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="92b29-111">Атрибут</span><span class="sxs-lookup"><span data-stu-id="92b29-111">Attribute</span></span>         | <span data-ttu-id="92b29-112">Тип</span><span class="sxs-lookup"><span data-stu-id="92b29-112">Type</span></span>                     | <span data-ttu-id="92b29-113">Описание</span><span class="sxs-lookup"><span data-stu-id="92b29-113">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="92b29-114">Person — сведения</span><span class="sxs-lookup"><span data-stu-id="92b29-114">person-details</span></span> | <span data-ttu-id="92b29-115">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="92b29-115">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="92b29-116">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="92b29-116">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="92b29-117">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="92b29-117">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="92b29-118">Объект Person, определенный Microsoft Graph, содержащий сведения, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="92b29-118">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="92b29-119">Person — изображение</span><span class="sxs-lookup"><span data-stu-id="92b29-119">person-image</span></span>   | <span data-ttu-id="92b29-120">PNG/JPG/SVG</span><span class="sxs-lookup"><span data-stu-id="92b29-120">png/jpg/svg</span></span>                    | <span data-ttu-id="92b29-121">Изображение, связанное с лицом, которое отображается в карточке.</span><span class="sxs-lookup"><span data-stu-id="92b29-121">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="92b29-122">inherit — Details</span><span class="sxs-lookup"><span data-stu-id="92b29-122">inherit-details</span></span>   | <span data-ttu-id="92b29-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="92b29-123">None.</span></span>                  | <span data-ttu-id="92b29-124">Позволяет пользователю просматривать родительское дерево по родительскому `mgt-person` дереву, чтобы компонент `person-details` использовал `person-image` то же и данные.</span><span class="sxs-lookup"><span data-stu-id="92b29-124">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="92b29-125">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="92b29-125">Templates</span></span>

<span data-ttu-id="92b29-126">Компонент Person Card использует [шаблоны](../templates.md) , позволяющие добавлять или заменять части компонента.</span><span class="sxs-lookup"><span data-stu-id="92b29-126">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="92b29-127">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="92b29-127">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="92b29-128">Тип данных</span><span class="sxs-lookup"><span data-stu-id="92b29-128">Data type</span></span> | <span data-ttu-id="92b29-129">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="92b29-129">Data context</span></span> | <span data-ttu-id="92b29-130">Описание</span><span class="sxs-lookup"><span data-stu-id="92b29-130">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="92b29-131">умолчани</span><span class="sxs-lookup"><span data-stu-id="92b29-131">default</span></span> | <span data-ttu-id="92b29-132">`person`: Объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="92b29-132">`person`: The person details object</span></span> <br> <span data-ttu-id="92b29-133">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="92b29-133">`personImage`: The URL of the image</span></span> | <span data-ttu-id="92b29-134">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="92b29-134">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="92b29-135">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="92b29-135">additional-details</span></span> | <span data-ttu-id="92b29-136">`person`: Объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="92b29-136">`person`: The person details object</span></span> <br> <span data-ttu-id="92b29-137">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="92b29-137">`personImage`: the URL of the image</span></span> | <span data-ttu-id="92b29-138">Шаблон, используемый для добавления в карточку дополнительного контента.</span><span class="sxs-lookup"><span data-stu-id="92b29-138">The template used to add additional content to the card.</span></span> |

<span data-ttu-id="92b29-139">Например, вы можете использовать шаблон для настройки компонента, присоединенного к `mgt-person` компоненту, и шаблона, чтобы добавить дополнительные сведения в карточку.</span><span class="sxs-lookup"><span data-stu-id="92b29-139">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card inherit-details>
          <template data-type="additional-details">
            <h3>Stuffed Animal Friends:</h3>
            <ul>
              <li>Giraffe</li>
              <li>lion</li>
              <li>Rabbit</li>
            </ul>
          </template>
        </mgt-person-card>
      </template>
    </mgt-person>

```

## <a name="css-custom-properties"></a><span data-ttu-id="92b29-140">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="92b29-140">CSS custom properties</span></span>

<span data-ttu-id="92b29-141">`mgt-person-card` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="92b29-141">The `mgt-person-card` component defines the following CSS custom properties.</span></span>

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

<span data-ttu-id="92b29-142">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="92b29-142">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="92b29-143">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="92b29-143">Microsoft Graph permissions</span></span>

<span data-ttu-id="92b29-144">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений.</span><span class="sxs-lookup"><span data-stu-id="92b29-144">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="92b29-145">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="92b29-145">Authentication</span></span>

<span data-ttu-id="92b29-146">В элементе управления Person Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="92b29-146">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
