---
title: Шаблоны в наборе инструментов Microsoft Graph
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 46a1f9b771f358de6099bf1266c10c4c1ebe0cb0
ms.sourcegitcommit: 1bc5a0c179dce57e90349610566fb86e1b5fbf95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/04/2020
ms.locfileid: "43144263"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="44522-103">Шаблоны в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="44522-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="44522-104">Используйте настраиваемые шаблоны для изменения содержимого компонента.</span><span class="sxs-lookup"><span data-stu-id="44522-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="44522-105">Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента.</span><span class="sxs-lookup"><span data-stu-id="44522-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="44522-106">Например, чтобы переопределить шаблон компонента, добавьте `<template>` элемент в компонент.</span><span class="sxs-lookup"><span data-stu-id="44522-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

## <a name="data-type"></a><span data-ttu-id="44522-107">Тип данных</span><span class="sxs-lookup"><span data-stu-id="44522-107">Data-type</span></span>

<span data-ttu-id="44522-108">Каждый компонент может иметь несколько частей, которые можно использовать в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="44522-108">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="44522-109">Например, в `mgt-agenda` компоненте можно зашаблонировать отдельные события, заголовки отдельных разделов, Загрузка представления, без представления данных и т. д.</span><span class="sxs-lookup"><span data-stu-id="44522-109">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="44522-110">Чтобы указать шаблон, используйте `data-type` атрибут для шаблона.</span><span class="sxs-lookup"><span data-stu-id="44522-110">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="44522-111">Например, чтобы указать шаблон для каждого события в `mgt-agenda`, используйте тип `event` данных, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="44522-111">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="44522-112">Если этот `data-type` параметр не указан, весь компонент будет заменен на шаблон.</span><span class="sxs-lookup"><span data-stu-id="44522-112">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="44522-113">Вы также можете использовать `data-type="default"` для этой цели.</span><span class="sxs-lookup"><span data-stu-id="44522-113">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="44522-114">Привязка данных</span><span class="sxs-lookup"><span data-stu-id="44522-114">Binding data</span></span>

<span data-ttu-id="44522-115">Многие шаблоны позволяют привязать данные, которые передаются шаблону в качестве контекста данных.</span><span class="sxs-lookup"><span data-stu-id="44522-115">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="44522-116">Например, `event` шаблон в `mgt-agenda` компоненте передает `{event}` объект, который можно использовать непосредственно в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="44522-116">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="44522-117">Чтобы развернуть выражение, например `event.subject`, используйте двойные фигурные скобки.</span><span class="sxs-lookup"><span data-stu-id="44522-117">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="44522-118">Этот формат также можно использовать в атрибутах:</span><span class="sxs-lookup"><span data-stu-id="44522-118">This format can also be used inside of attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="44522-119">**Примечание:** Вы также можете развернуть такие объекты, `{{event}}` как, и они будут отображаться как строки JSON.</span><span class="sxs-lookup"><span data-stu-id="44522-119">**Note:** You can also expand objects such as `{{event}}` and they will render as JSON strings.</span></span> <span data-ttu-id="44522-120">Это может быть удобно при разработке шаблонов.</span><span class="sxs-lookup"><span data-stu-id="44522-120">This can be useful when you're developing the templates.</span></span>

## <a name="data-context-helper-properties"></a><span data-ttu-id="44522-121">Вспомогательные свойства контекста данных</span><span class="sxs-lookup"><span data-stu-id="44522-121">Data context helper properties</span></span>

<span data-ttu-id="44522-122">Следующие свойства также можно использовать с объектом контекста данных в шаблонах.</span><span class="sxs-lookup"><span data-stu-id="44522-122">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="44522-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="44522-123">Property</span></span> |  <span data-ttu-id="44522-124">Описание</span><span class="sxs-lookup"><span data-stu-id="44522-124">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="44522-125">$index</span><span class="sxs-lookup"><span data-stu-id="44522-125">$index</span></span> | <span data-ttu-id="44522-126">Числовой индекс элемента, отображаемого в `data-for`цикле.</span><span class="sxs-lookup"><span data-stu-id="44522-126">Numerical index of item being rendered while being looped with `data-for`.</span></span> |
| <span data-ttu-id="44522-127">$parent</span><span class="sxs-lookup"><span data-stu-id="44522-127">$parent</span></span> | <span data-ttu-id="44522-128">Если шаблон отображается в другом шаблоне, это свойство позволяет получить доступ к родительскому контексту данных.</span><span class="sxs-lookup"><span data-stu-id="44522-128">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="44522-129">В приведенном ниже примере показано, как `$index` использовать свойство в цикле обработки данных.</span><span class="sxs-lookup"><span data-stu-id="44522-129">The following example shows how to use the `$index` property in a data-for loop.</span></span>

```html
<mgt-person>
  <mgt-person-card>
    <template data-type="additional-details">
      <span data-for="language in languages">
        {{ language.displayName }}<span data-if="$index < languages.length - 1">, </span>
      </span>
    </template>
  </mgt-person-card>
</mgt-person>
```

## <a name="conditional-rendering"></a><span data-ttu-id="44522-130">Условная визуализация</span><span class="sxs-lookup"><span data-stu-id="44522-130">Conditional rendering</span></span>

<span data-ttu-id="44522-131">Вы можете отображать элементы только в том случае, если условие имеет значение true или false в зависимости от контекста данных.</span><span class="sxs-lookup"><span data-stu-id="44522-131">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="44522-132">Атрибуты `data-if` и `data-else` могут оценивать выражение и отображать только значения true и false.</span><span class="sxs-lookup"><span data-stu-id="44522-132">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="44522-133">Циклов</span><span class="sxs-lookup"><span data-stu-id="44522-133">Looping</span></span>

<span data-ttu-id="44522-134">Существуют случаи, когда объект контекста данных содержит цикл, и вам потребуется перебрать данные.</span><span class="sxs-lookup"><span data-stu-id="44522-134">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="44522-135">В этом случае используйте `data-for` атрибут.</span><span class="sxs-lookup"><span data-stu-id="44522-135">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="templatecontext"></a><span data-ttu-id="44522-136">темплатеконтекст</span><span class="sxs-lookup"><span data-stu-id="44522-136">TemplateContext</span></span>

<span data-ttu-id="44522-137">Каждый компонент в наборе инструментов Microsoft Graph определяет `templateContext` свойство, которое можно использовать для передачи дополнительных данных в любой шаблон компонента.</span><span class="sxs-lookup"><span data-stu-id="44522-137">Each component in the Microsoft Graph Toolkit defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span> 

```ts
document.querySelector('mgt-agenda').templateContext = {

  someObject: {},
  formatDate: (date: Date) => { /* format date and return */ },
  someEventHandler: (e) => { /* handleEvent */  }

}
```

<span data-ttu-id="44522-138">Теперь свойства `templateContext` объекта станут доступны для использования в выражениях привязки в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="44522-138">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

<span data-ttu-id="44522-139">Это может быть полезен во многих сценариях, таких как преобразование данных в привязки или привязывание к событиям.</span><span class="sxs-lookup"><span data-stu-id="44522-139">This can be useful in many scenarios, such as converting data in your bindings, or binding to events.</span></span> 

### <a name="converters"></a><span data-ttu-id="44522-140">Типов</span><span class="sxs-lookup"><span data-stu-id="44522-140">Converters</span></span>

<span data-ttu-id="44522-141">Во многих случаях может потребоваться преобразовать данные перед их представлением в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="44522-141">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="44522-142">Например, вам может потребоваться правильно отформатировать дату перед отображением.</span><span class="sxs-lookup"><span data-stu-id="44522-142">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="44522-143">В таких случаях может потребоваться использование конвертера шаблонов.</span><span class="sxs-lookup"><span data-stu-id="44522-143">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="44522-144">Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет выполнять преобразование.</span><span class="sxs-lookup"><span data-stu-id="44522-144">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="44522-145">Например, вы можете определить функцию для преобразования объекта события в отформатированный диапазон времени.</span><span class="sxs-lookup"><span data-stu-id="44522-145">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="44522-146">Чтобы использовать конвертер в шаблоне, используйте его, как если бы вы использовали функцию в коде программной части.</span><span class="sxs-lookup"><span data-stu-id="44522-146">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="44522-147">Привязка события или свойства</span><span class="sxs-lookup"><span data-stu-id="44522-147">Event or property binding</span></span>

<span data-ttu-id="44522-148">`data-props` Атрибут позволяет добавить прослушиватель событий или задать значение свойства непосредственно в шаблонах.</span><span class="sxs-lookup"><span data-stu-id="44522-148">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span> 

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="44522-149">Свойства Data/PROPS принимают строку с разделителями запятыми для каждого свойства или обработчика событий, который может потребоваться задать.</span><span class="sxs-lookup"><span data-stu-id="44522-149">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span> 

<span data-ttu-id="44522-150">Чтобы добавить обработчик событий, добавьте к имени события префикс `@`.</span><span class="sxs-lookup"><span data-stu-id="44522-150">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="44522-151">Обработчик события должен быть доступен в `templateContext` элементе.</span><span class="sxs-lookup"><span data-stu-id="44522-151">The event handler will need to be available in the `templateContext` of the element.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  someEventHandler: (e, context, root) => { /* handleEvent */  }

}
```

```html
<template>
    <button data-props="{{@click: someEventHandler}}"></button>
</template>
```

<span data-ttu-id="44522-152">Аргументы события, контекст данных и корневой элемент шаблона передаются обработчику событий в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="44522-152">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="44522-153">Событие, отображаемое в шаблоне</span><span class="sxs-lookup"><span data-stu-id="44522-153">Template rendered event</span></span>

<span data-ttu-id="44522-154">В некоторых случаях может потребоваться получить ссылку на визуализированный элемент.</span><span class="sxs-lookup"><span data-stu-id="44522-154">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="44522-155">Это может быть удобно, если вы хотите самостоятельно обработать отображение контента или изменить отображаемый элемент.</span><span class="sxs-lookup"><span data-stu-id="44522-155">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="44522-156">В этом сценарии можно использовать `templateRendered` событие, которое срабатывает после отображения шаблона.</span><span class="sxs-lookup"><span data-stu-id="44522-156">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="44522-157">Сведения о событии будут содержать ссылку на отображаемый элемент, объект контекста данных и тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="44522-157">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

```ts
agenda.addEventListener('templateRendered', (e) => { 
  let templateType = e.detail.templateType;
  let dataContext = e.detail.context;
  let element = e.detail.element;

  if (templateType === 'event') {
    element.querySelector('.some-button').addEventListener('click', () => {});
  }
});
```

## <a name="styling"></a><span data-ttu-id="44522-158">Изменении</span><span class="sxs-lookup"><span data-stu-id="44522-158">Styling</span></span>

<span data-ttu-id="44522-159">Шаблоны можно обычно отформатировать с помощью CSS, так как они отображаются вне теневой модели DOM.</span><span class="sxs-lookup"><span data-stu-id="44522-159">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
