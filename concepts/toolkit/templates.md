---
title: Шаблоны в наборе инструментов Microsoft Graph
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b9ef4b9422d84886fa4df76618b6cdf14def2378
ms.sourcegitcommit: d9e94c109c0934cc93f340aafa1dccaa1a5da9c7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37275712"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="ff4fb-103">Шаблоны в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ff4fb-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="ff4fb-104">Используйте настраиваемые шаблоны для изменения содержимого компонента.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="ff4fb-105">Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="ff4fb-106">Например, чтобы переопределить шаблон компонента, добавьте `<template>` элемент в компонент.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

## <a name="data-type"></a><span data-ttu-id="ff4fb-107">Тип данных</span><span class="sxs-lookup"><span data-stu-id="ff4fb-107">Data-type</span></span>

<span data-ttu-id="ff4fb-108">Каждый компонент может иметь несколько частей, которые можно использовать в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-108">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="ff4fb-109">Например, в `mgt-agenda` компоненте можно зашаблонировать отдельные события, заголовки отдельных разделов, Загрузка представления, без представления данных и т. д.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-109">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="ff4fb-110">Чтобы указать шаблон, используйте `data-type` атрибут для шаблона.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-110">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="ff4fb-111">Например, чтобы указать шаблон для каждого события в `mgt-agenda`, используйте тип `event` данных, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-111">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="ff4fb-112">Если этот `data-type` параметр не указан, весь компонент будет заменен на шаблон.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-112">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="ff4fb-113">Вы также можете использовать `data-type="default"` для этой цели.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-113">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="ff4fb-114">Привязка данных</span><span class="sxs-lookup"><span data-stu-id="ff4fb-114">Binding data</span></span>

<span data-ttu-id="ff4fb-115">Многие шаблоны позволяют привязать данные, которые передаются шаблону в качестве контекста данных.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-115">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="ff4fb-116">Например, `event` шаблон в `mgt-agenda` компоненте передает `{event}` объект, который можно использовать непосредственно в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-116">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="ff4fb-117">Чтобы развернуть выражение, например `event.subject`, используйте двойные фигурные скобки.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-117">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="ff4fb-118">Этот формат также можно использовать в атрибутах:</span><span class="sxs-lookup"><span data-stu-id="ff4fb-118">This format can also be used inside of attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="ff4fb-119">**Примечание:** Вы также можете развернуть такие объекты, `{{event}}` как, и они будут отображаться как строки JSON.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-119">**Note:** You can also expand objects such as `{{event}}` and they will render as JSON strings.</span></span> <span data-ttu-id="ff4fb-120">Это может быть удобно при разработке шаблонов.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-120">This can be useful when you're developing the templates.</span></span>

## <a name="conditional-rendering"></a><span data-ttu-id="ff4fb-121">Условная визуализация</span><span class="sxs-lookup"><span data-stu-id="ff4fb-121">Conditional rendering</span></span>

<span data-ttu-id="ff4fb-122">Вы можете отображать элементы только в том случае, если условие имеет значение true или false в зависимости от контекста данных.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-122">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="ff4fb-123">Атрибуты `data-if` и `data-else` могут оценивать выражение и отображать только значения true и false.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-123">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

```html
<mgt-person person-query="john doe">
  <template>
    <div data-if="person.image">
      <img src="{{ person.image }}" />
    </div>
    <div data-else>
      {{ person.displayName }}
    </div>
  </template>
</mgt-person>
```

## <a name="looping"></a><span data-ttu-id="ff4fb-124">Циклов</span><span class="sxs-lookup"><span data-stu-id="ff4fb-124">Looping</span></span>

<span data-ttu-id="ff4fb-125">Существуют случаи, когда объект контекста данных содержит цикл, и вам потребуется перебрать данные.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-125">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="ff4fb-126">В этом случае используйте `data-for` атрибут.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-126">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="converters"></a><span data-ttu-id="ff4fb-127">Типов</span><span class="sxs-lookup"><span data-stu-id="ff4fb-127">Converters</span></span>

<span data-ttu-id="ff4fb-128">Во многих случаях может потребоваться преобразовать данные перед их представлением в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-128">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="ff4fb-129">Например, вам может потребоваться правильно отформатировать дату перед отображением.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-129">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="ff4fb-130">В таких случаях может потребоваться использование конвертера шаблонов.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-130">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="ff4fb-131">Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет выполнять преобразование.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-131">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="ff4fb-132">Например, вы можете определить функцию для форматирования даты.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-132">For example, you might define a function to format a date.</span></span>

```ts
getTimeRange(event) {
  // TODO: format a string from the event object as you wish
  // timeRange = ...

  return timeRange;
}
```

<span data-ttu-id="ff4fb-133">Затем определите новый конвертер для элемента и присвойте ему имя по своему усмотрению.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-133">Then define a new converter on the element and name it as you see fit.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.templateConverters["myConverter"] = getTimeRange;
```

<span data-ttu-id="ff4fb-134">Чтобы использовать конвертер в шаблоне, используйте тройные фигурные скобки.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-134">To use the converter in your template, use the triple curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{{ myConverter(event) }}}</div>
</template>
```

<span data-ttu-id="ff4fb-135">Вы также можете использовать встроенные функции, не определяя Конвертер шаблонов.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-135">You can also use built-in functions without defining template converter.</span></span>

```html
<template data-type="event">
  <div>{{{ event.subject.toUpperCase() }}}</div>
</template>
```

## <a name="template-rendered-event"></a><span data-ttu-id="ff4fb-136">Событие, отображаемое в шаблоне</span><span class="sxs-lookup"><span data-stu-id="ff4fb-136">Template Rendered Event</span></span>

<span data-ttu-id="ff4fb-137">В некоторых случаях может потребоваться получить ссылку на визуализированный элемент.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-137">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="ff4fb-138">Это может быть удобно для добавления прослушивателей событий в элементы шаблона.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-138">This can be useful for adding event listeners to elements in the template.</span></span> <span data-ttu-id="ff4fb-139">В этом случае вы можете использовать `templateRendered` событие.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-139">In this scenario, you might use the `templateRendered` event.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="ff4fb-140">Сведения о событии будут содержать ссылку на отображаемый элемент, объект контекста данных и тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-140">The event details will contain reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

```ts
agenda.addEventListener('templateRendered', (e) => { 
  let templateType = e.detail.templateType;
  let dataContext = e.detail.context;
  let element = e.detail.element;

  if (type === 'event') {
    element.querySelector('.some-button').addEventListener('click', () => {});
  }
});
```

## <a name="styling"></a><span data-ttu-id="ff4fb-141">Изменении</span><span class="sxs-lookup"><span data-stu-id="ff4fb-141">Styling</span></span>

<span data-ttu-id="ff4fb-142">Шаблоны можно обычно отформатировать с помощью CSS, так как они отображаются вне теневой модели DOM.</span><span class="sxs-lookup"><span data-stu-id="ff4fb-142">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
