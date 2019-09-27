---
title: Компонент Person Card в наборе инструментов Microsoft Graph
description: Компонент Person-Card является компонентом для отображения дополнительных сведений, относящихся к пользователю.
localization_priority: Normal
author: vogtn
ms.openlocfilehash: f4d8c975fe91d91658f512cea708ee104d4fd906
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275859"
---
# <a name="person-card-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="fba47-103">Компонент Person Card в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fba47-103">Person-Card component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="fba47-104">Компонент Person-Card — это реагирующий на работу компонент для отображения дополнительных сведений, относящихся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="fba47-104">A Person-Card component is a responsive component to display more information related to a person.</span></span> <span data-ttu-id="fba47-105">Он обычно используется в качестве всплывающего элемента в `mgt-person` компоненте.</span><span class="sxs-lookup"><span data-stu-id="fba47-105">It is generally used as a flyout on the `mgt-person` component.</span></span>

<span data-ttu-id="fba47-106">Дополнительную информацию о компоненте `mgt-person` можно узнать в статье [упр](./person.md).</span><span class="sxs-lookup"><span data-stu-id="fba47-106">For more information about the `mgt-person` component, see [mgt-person docs](./person.md).</span></span>
  
## <a name="example"></a><span data-ttu-id="fba47-107">Пример</span><span class="sxs-lookup"><span data-stu-id="fba47-107">Example</span></span>

```html
<mgt-person-card person-details="{personObject}" person-image="imgUrl"></mgt-person-card>
```

## <a name="properties"></a><span data-ttu-id="fba47-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fba47-108">Properties</span></span>

<span data-ttu-id="fba47-109">Компонент использует Microsoft Graph для предоставления дополнительных сведений о пользователе.</span><span class="sxs-lookup"><span data-stu-id="fba47-109">The component uses Microsoft Graph to provide additional details about the user.</span></span> <span data-ttu-id="fba47-110">Чтобы определить пользователя, необходимо использовать свойство **Person — запрос** `mgt-person`.</span><span class="sxs-lookup"><span data-stu-id="fba47-110">To define a user, you must use the **person-query** property of `mgt-person`.</span></span>

| <span data-ttu-id="fba47-111">Атрибут</span><span class="sxs-lookup"><span data-stu-id="fba47-111">Attribute</span></span>         | <span data-ttu-id="fba47-112">type</span><span class="sxs-lookup"><span data-stu-id="fba47-112">type</span></span>                     | <span data-ttu-id="fba47-113">Описание</span><span class="sxs-lookup"><span data-stu-id="fba47-113">Description</span></span>                                                                           |
| ---------------- | -------------------------------- | ------------------------------------------------------------------------------------- |
| <span data-ttu-id="fba47-114">Person — сведения</span><span class="sxs-lookup"><span data-stu-id="fba47-114">person-details</span></span> | <span data-ttu-id="fba47-115">MicrosoftGraph. User</span><span class="sxs-lookup"><span data-stu-id="fba47-115">MicrosoftGraph.User</span></span> <br> <span data-ttu-id="fba47-116">MicrosoftGraph. Person</span><span class="sxs-lookup"><span data-stu-id="fba47-116">MicrosoftGraph.Person</span></span> <br> <span data-ttu-id="fba47-117">MicrosoftGraph. Contact</span><span class="sxs-lookup"><span data-stu-id="fba47-117">MicrosoftGraph.Contact</span></span> | <span data-ttu-id="fba47-118">Объект Person, определенный Microsoft Graph, содержащий сведения, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="fba47-118">Person object as defined by Microsoft Graph, containing details related to the user.</span></span> |
| <span data-ttu-id="fba47-119">Person — изображение</span><span class="sxs-lookup"><span data-stu-id="fba47-119">person-image</span></span>   | <span data-ttu-id="fba47-120">PNG/JPG/SVG</span><span class="sxs-lookup"><span data-stu-id="fba47-120">png/jpg/svg</span></span>                    | <span data-ttu-id="fba47-121">Изображение, связанное с лицом, которое отображается в карточке.</span><span class="sxs-lookup"><span data-stu-id="fba47-121">Image related to the person displayed in the card.</span></span>                                   |



## <a name="templates"></a><span data-ttu-id="fba47-122">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="fba47-122">Templates</span></span>

<span data-ttu-id="fba47-123">Компонент Person Card использует [шаблоны](../templates.md) , позволяющие добавлять или заменять части компонента.</span><span class="sxs-lookup"><span data-stu-id="fba47-123">The Person-Card component uses [templates](../templates.md) that allow you to add or replace portions of the component.</span></span> <span data-ttu-id="fba47-124">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="fba47-124">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following.</span></span>

| <span data-ttu-id="fba47-125">Тип данных</span><span class="sxs-lookup"><span data-stu-id="fba47-125">Data type</span></span> | <span data-ttu-id="fba47-126">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="fba47-126">Data context</span></span> | <span data-ttu-id="fba47-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fba47-127">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="fba47-128">умолчани</span><span class="sxs-lookup"><span data-stu-id="fba47-128">default</span></span> | <span data-ttu-id="fba47-129">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="fba47-129">person: The person details object</span></span> <br> <span data-ttu-id="fba47-130">Персонимаже: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="fba47-130">personImage: The URL of the image</span></span> | <span data-ttu-id="fba47-131">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="fba47-131">The default template replaces the entire component with your own.</span></span> |
| <span data-ttu-id="fba47-132">Дополнительные сведения</span><span class="sxs-lookup"><span data-stu-id="fba47-132">additional-details</span></span> | <span data-ttu-id="fba47-133">Person: объект сведений о лице</span><span class="sxs-lookup"><span data-stu-id="fba47-133">person: The person details object</span></span> <br> <span data-ttu-id="fba47-134">Персонимаже: URL-адрес изображения</span><span class="sxs-lookup"><span data-stu-id="fba47-134">personImage: the URL of the image</span></span> | <span data-ttu-id="fba47-135">Шаблон, используемый для добавления в карточку дополнительного контента.</span><span class="sxs-lookup"><span data-stu-id="fba47-135">The template used to add additional content to the card.</span></span> |

<span data-ttu-id="fba47-136">Например, вы можете использовать шаблон для настройки компонента, присоединенного к `mgt-person` компоненту, и шаблона, чтобы добавить дополнительные сведения в карточку.</span><span class="sxs-lookup"><span data-stu-id="fba47-136">For example, you can use a template to customize the component attached to the `mgt-person` component and a template to add additional details in the card.</span></span> 

```html
    <mgt-person person-query="me" show-name show-email person-card="hover">
      <template data-type="person-card">
        <mgt-person-card person-details="{{person}}" 
            person-image="{{personImage}}">
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

## <a name="css-custom-properties"></a><span data-ttu-id="fba47-137">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="fba47-137">CSS custom properties</span></span>

<span data-ttu-id="fba47-138">`mgt-person-card` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="fba47-138">The `mgt-person-card` component defines the following CSS custom properties.</span></span>

```css
mgt-person-card {
  --font-size: 14px;
  --font-weight: 600;
  --height: '100%';
  --background-color: transparent;
}
```

<span data-ttu-id="fba47-139">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="fba47-139">To learn more, see [styling components](../style.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="fba47-140">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="fba47-140">Microsoft Graph permissions</span></span>

<span data-ttu-id="fba47-141">Этот компонент использует [компонент Person](./person.md) для отображения пользователя и наследования всех разрешений.</span><span class="sxs-lookup"><span data-stu-id="fba47-141">This component uses the [Person component](./person.md) to display the user and inherits all permissions.</span></span> 

## <a name="authentication"></a><span data-ttu-id="fba47-142">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="fba47-142">Authentication</span></span>

<span data-ttu-id="fba47-143">В элементе управления Person Card используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="fba47-143">The Person-Card control uses the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 
