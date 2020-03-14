---
title: Компонент Person Card в наборе инструментов Microsoft Graph
description: Компонент Person-Card является компонентом для отображения дополнительных сведений, относящихся к пользователю.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: 336e6beabc227a2574e41cf6a658d38fdabfcdcf
ms.sourcegitcommit: f2dffaca3e1c5b74a01b59e1b76dba1592a6a5d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/14/2020
ms.locfileid: "42639928"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="774ed-103">Компонент Person Card в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="774ed-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="774ed-104">Компонент Person-Card — это реагирующий на работу компонент для отображения дополнительных сведений, относящихся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="774ed-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="774ed-105">Он обычно используется в качестве всплывающего элемента в `mgt-person` компоненте.</span><span class="sxs-lookup"><span data-stu-id="774ed-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="774ed-106">Дополнительную информацию о компоненте `mgt-person` можно узнать в статье [упр](./person.md).</span><span class="sxs-lookup"><span data-stu-id="774ed-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>

## <a name="example"></a><span data-ttu-id="774ed-107">Пример</span><span class="sxs-lookup"><span data-stu-id="774ed-107">Example</span></span>

<span data-ttu-id="774ed-108">В следующем примере показано использование `mgt-person-card` компонента с `mgt-person` компонентом.</span><span class="sxs-lookup"><span data-stu-id="774ed-108">The following example shows the use of the `mgt-person-card` component with a `mgt-person` component.</span></span> <span data-ttu-id="774ed-109">Наведите указатель мыши на лицо, чтобы увидеть карточку сотрудника, и используйте редактор кода, чтобы увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="774ed-109">Hover over the person to see the Person Card and use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>
  
<iframe src="https://mgt.dev/iframe.html?id=components-mgt-person-card--person-card-hover&source=docs" height="400"></iframe>

[<span data-ttu-id="774ed-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="774ed-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-person-card--person-card-hover&source=docs)

## <a name="properties"></a><span data-ttu-id="774ed-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="774ed-111">Properties</span></span>

<span data-ttu-id="774ed-112">Компонент использует Microsoft Graph для предоставления дополнительных сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="774ed-112">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="774ed-113">Чтобы определить пользователя, необходимо использовать свойство **Person — запрос** `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="774ed-113">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="774ed-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="774ed-114">Attribute</span></span>         | <span data-ttu-id="774ed-115">Тип</span><span class="sxs-lookup"><span data-stu-id="774ed-115">Type</span></span>                     | <span data-ttu-id="774ed-116">Описание</span><span class="sxs-lookup"><span data-stu-id="774ed-116">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="774ed-117">Person — сведения</span><span class="sxs-lookup"><span data-stu-id="774ed-117">person-details</span></span> | <span data-ttu-id="774ed-118">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="774ed-118">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="774ed-119">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="774ed-119">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="774ed-120">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="774ed-120">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="774ed-121">Объект Person, определенный Microsoft Graph, содержащий сведения, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="774ed-121">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="774ed-122">Person — изображение</span><span class="sxs-lookup"><span data-stu-id="774ed-122">person-image</span></span>   | <span data-ttu-id="774ed-123">PNG/JPG/SVG</span><span class="sxs-lookup"><span data-stu-id="774ed-123">png/jpg/svg</span></span>                    | <span data-ttu-id="774ed-124">Изображение, связанное с лицом, которое отображается в карточке.</span><span class="sxs-lookup"><span data-stu-id="774ed-124">Image related to the person displayed in the card.</span></span>                                   |
| <span data-ttu-id="774ed-125">inherit — Details</span><span class="sxs-lookup"><span data-stu-id="774ed-125">inherit-details</span></span>   | <span data-ttu-id="774ed-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="774ed-126">None.</span></span>                  | <span data-ttu-id="774ed-127">Позволяет пользователю просматривать родительское дерево по родительскому `mgt-person` дереву, чтобы компонент `person-details` использовал `person-image` то же и данные.</span><span class="sxs-lookup"><span data-stu-id="774ed-127">Allows person-card to walk parent tree for `mgt-person` component to use the same `person-details` and `person-image` data.</span></span>                      |


## <a name="templates"></a><span data-ttu-id="774ed-128">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="774ed-128">Templates</span></span>

<span data-ttu-id="774ed-129">Компонент Person Card использует [шаблоны](../templates.md) , позволяющие добавлять или заменять части компонента.</span><span class="sxs-lookup"><span data-stu-id="774ed-129">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="774ed-130">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="774ed-130">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="774ed-131">Тип данных</span><span class="sxs-lookup"><span data-stu-id="774ed-131">Data type</span></span> | <span data-ttu-id="774ed-132">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="774ed-132">Data context</span></span> | <span data-ttu-id="774ed-133">Описание</span><span class="sxs-lookup"><span data-stu-id="774ed-133">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="774ed-134">умолчани</span><span class="sxs-lookup"><span data-stu-id="774ed-134">default</span></span> | <span data-ttu-id="774ed-135">`person`: Объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="774ed-135">`person`: The person details object</span></span> <br> <span data-ttu-id="774ed-136">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="774ed-136">`personImage`: The URL of the image</span></span> | <span data-ttu-id="774ed-137">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="774ed-137">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="774ed-138">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="774ed-138">additional-details</span></span> | <span data-ttu-id="774ed-139">`person`: Объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="774ed-139">`person`: The person details object</span></span> <br> <span data-ttu-id="774ed-140">`personImage`: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="774ed-140">`personImage`: the URL of the image</span></span> | <span data-ttu-id="774ed-141">Шаблон, используемый для добавления в карточку дополнительного контента.</span><span class="sxs-lookup"><span data-stu-id="774ed-141">The template used to add additional content to the card.</span></span> |

<span data-ttu-id="774ed-142">Например, вы можете использовать шаблон для настройки компонента, присоединенного к `mgt-person` компоненту, и шаблона, чтобы добавить дополнительные сведения в карточку.</span><span class="sxs-lookup"><span data-stu-id="774ed-142">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

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

## <a name="css-custom-properties"></a><span data-ttu-id="774ed-143">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="774ed-143">CSS custom properties</span></span>

<span data-ttu-id="774ed-144">`mgt-person-card` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="774ed-144">The `mgt-person-card` component defines the following CSS custom properties.</span></span>

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

<span data-ttu-id="774ed-145">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="774ed-145">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="774ed-146">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="774ed-146">Microsoft Graph permissions</span></span>

<span data-ttu-id="774ed-147">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений.</span><span class="sxs-lookup"><span data-stu-id="774ed-147">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="774ed-148">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="774ed-148">Authentication</span></span>

<span data-ttu-id="774ed-149">В элементе управления Person Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="774ed-149">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
