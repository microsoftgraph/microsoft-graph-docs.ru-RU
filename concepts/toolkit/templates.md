---
title: Шаблоны в наборе инструментов Microsoft Graph
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: f0648d0ac1348fbadad6cebe8a022f9445fcf1e3
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243069"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="cf963-103">Шаблоны в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="cf963-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="cf963-104">Используйте настраиваемые шаблоны для изменения содержимого компонента.</span><span class="sxs-lookup"><span data-stu-id="cf963-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="cf963-105">Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента.</span><span class="sxs-lookup"><span data-stu-id="cf963-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="cf963-106">Например, чтобы переопределить шаблон компонента, добавьте `<template>` элемент в компонент.</span><span class="sxs-lookup"><span data-stu-id="cf963-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

```html
<mgt-agenda>
  <template data-type="event">
      <div>{{event.subject}}</div>
      <div data-for='attendee in event.attendees'>
          <mgt-person person-query="{{attendee.emailAddress.name}}">
            <template>
              <div data-if="person.image">
                <img src="{{person.image}}" />
              </div>
              <div data-else>
                {{person.displayName}}
              </div>
            </template>
          </mgt-person>
      </div>
  </template>
</mgt-agenda>
```

<span data-ttu-id="cf963-107">Поддерживаются следующие функции шаблонов:</span><span class="sxs-lookup"><span data-stu-id="cf963-107">The following template features are supported:</span></span>

- <span data-ttu-id="cf963-108">Используйте двойные фигурные скобки`{{expression}}`(), чтобы развернуть выражение.</span><span class="sxs-lookup"><span data-stu-id="cf963-108">Use the double curly brackets (`{{expression}}`) to expand an expression.</span></span> <span data-ttu-id="cf963-109">В предыдущем примере `<mgt-person>` `person` объект передает объект, который можно использовать в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="cf963-109">In the previous example, the `<mgt-person>` passes a `person` object that you can use in the template.</span></span>
- <span data-ttu-id="cf963-110">Используйте атрибуты `data-if` и `data-else` для условной визуализации.</span><span class="sxs-lookup"><span data-stu-id="cf963-110">Use the `data-if` and `data-else` attributes for conditional rendering.</span></span> <span data-ttu-id="cf963-111">Условные выражения, `event.attendees.length > 2` такие как, поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="cf963-111">Conditional expressions such as `event.attendees.length > 2` are supported.</span></span>
- <span data-ttu-id="cf963-112">Используйте `data-for` для повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="cf963-112">Use the `data-for` to repeat an element.</span></span>
- <span data-ttu-id="cf963-113">Используйте параметр `data-type` для указания части компонента, к которой следует применить шаблон.</span><span class="sxs-lookup"><span data-stu-id="cf963-113">Use the `data-type` to specify what part of the component to template.</span></span> <span data-ttu-id="cf963-114">Если не указать тип, шаблон будет применен ко всему компоненту.</span><span class="sxs-lookup"><span data-stu-id="cf963-114">Not specifying the type will apply the template to the entire component.</span></span>

<span data-ttu-id="cf963-115">Каждый компонент документирует поддерживаемые `data-type` значения и контекст данных, передаваемых по шаблону.</span><span class="sxs-lookup"><span data-stu-id="cf963-115">Each component documents the supported `data-type` values and what data context is passed down to each template.</span></span>

<span data-ttu-id="cf963-116">Шаблоны можно использовать в обычном стиле, так как они отображаются вне теневой модели DOM.</span><span class="sxs-lookup"><span data-stu-id="cf963-116">The templates can be styled normally as they are rendered outside of the shadow dom.</span></span>
