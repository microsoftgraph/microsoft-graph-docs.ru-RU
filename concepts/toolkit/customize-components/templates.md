---
title: Шаблоны в microsoft Graph набор средств
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 94529f45c95dcfdd56ade2dffc7b4ac7bf48babb
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658592"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="5ff48-103">Шаблоны в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="5ff48-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="5ff48-104">Большинство компонентов набор средств Microsoft Graph поддерживают использование настраиваемого шаблона для изменения содержимого компонента.</span><span class="sxs-lookup"><span data-stu-id="5ff48-104">Most Microsoft Graph Toolkit components support the use of custom templates to modify the content of a component.</span></span>

<span data-ttu-id="5ff48-105">Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента.</span><span class="sxs-lookup"><span data-stu-id="5ff48-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="5ff48-106">Например, чтобы переопредить шаблон компонента, добавьте `<template>` элемент внутри компонента.</span><span class="sxs-lookup"><span data-stu-id="5ff48-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

<span data-ttu-id="5ff48-107">Если вы используете компоненты Microsoft Graph набор средств React, вы можете использовать React для оформления шаблонов.</span><span class="sxs-lookup"><span data-stu-id="5ff48-107">If you're using the Microsoft Graph Toolkit React components, you can use React for authoring templates.</span></span> <span data-ttu-id="5ff48-108">Подробные сведения [см. в этом наборе инструментов с React.](../get-started/mgt-react.md)</span><span class="sxs-lookup"><span data-stu-id="5ff48-108">For details, see [Use the toolkit with React](../get-started/mgt-react.md).</span></span>

## <a name="data-type"></a><span data-ttu-id="5ff48-109">Тип данных</span><span class="sxs-lookup"><span data-stu-id="5ff48-109">Data-type</span></span>

<span data-ttu-id="5ff48-110">Каждый компонент может иметь несколько частей, которые могут быть шаблоны.</span><span class="sxs-lookup"><span data-stu-id="5ff48-110">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="5ff48-111">Например, в компоненте можно шаблонить отдельные события, отдельные разделы, представление загрузки, без представления `mgt-agenda` данных и т. д.</span><span class="sxs-lookup"><span data-stu-id="5ff48-111">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="5ff48-112">Чтобы указать шаблон, используйте `data-type` атрибут в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="5ff48-112">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="5ff48-113">Например, для шаблона каждого события в `mgt-agenda` , используйте `event` тип данных, как показано.</span><span class="sxs-lookup"><span data-stu-id="5ff48-113">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="5ff48-114">Если не `data-type` указано, весь компонент будет заменен шаблоном.</span><span class="sxs-lookup"><span data-stu-id="5ff48-114">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="5ff48-115">Вы также можете `data-type="default"` использовать для той же цели.</span><span class="sxs-lookup"><span data-stu-id="5ff48-115">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="5ff48-116">Привязка данных</span><span class="sxs-lookup"><span data-stu-id="5ff48-116">Binding data</span></span>

<span data-ttu-id="5ff48-117">Многие шаблоны позволяют привязыть данные, которые передаются в шаблон в качестве контекста данных.</span><span class="sxs-lookup"><span data-stu-id="5ff48-117">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="5ff48-118">Например, шаблон в компоненте передает объект, который `event` можно использовать непосредственно в `mgt-agenda` `{event}` шаблоне.</span><span class="sxs-lookup"><span data-stu-id="5ff48-118">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="5ff48-119">Чтобы развернуть выражение, `event.subject` например, используйте двойные фигурные скобки.</span><span class="sxs-lookup"><span data-stu-id="5ff48-119">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="5ff48-120">Этот формат также можно использовать в атрибутах:</span><span class="sxs-lookup"><span data-stu-id="5ff48-120">This format can also be used inside attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="5ff48-121">**Примечание.** Вы также можете развернуть такие объекты, как или они `{{event}}` будут отрисовыты `{{this}}` в качестве строк JSON.</span><span class="sxs-lookup"><span data-stu-id="5ff48-121">**Note:** You can also expand objects such as `{{event}}` or `{{this}}` and they will render as JSON strings.</span></span> <span data-ttu-id="5ff48-122">Это может быть полезно при разработке шаблонов.</span><span class="sxs-lookup"><span data-stu-id="5ff48-122">This can be useful when you're developing the templates.</span></span>

### <a name="change-binding-syntax"></a><span data-ttu-id="5ff48-123">Изменение синтаксиса привязки</span><span class="sxs-lookup"><span data-stu-id="5ff48-123">Change binding syntax</span></span>

<span data-ttu-id="5ff48-124">По умолчанию для расширения выражения используются двойные фигурные скобки ( `{{expression}}` ).</span><span class="sxs-lookup"><span data-stu-id="5ff48-124">By default, to expand an expression, you use double curly brackets ( `{{expression}}` ).</span></span> <span data-ttu-id="5ff48-125">Однако можно изменить этот синтаксис для сред, где уже используется синтаксис двойных фигурных скобок.</span><span class="sxs-lookup"><span data-stu-id="5ff48-125">However, you can change this syntax for environments where the double curly bracket syntax is already used.</span></span> <span data-ttu-id="5ff48-126">Например, в следующем примере используются двойные квадратные скобки ( `[[expression]]` ).</span><span class="sxs-lookup"><span data-stu-id="5ff48-126">For example, the following example uses double square brackets ( `[[expression]]` ).</span></span>

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a><span data-ttu-id="5ff48-127">Свойства помощника для контекста данных</span><span class="sxs-lookup"><span data-stu-id="5ff48-127">Data context helper properties</span></span>

<span data-ttu-id="5ff48-128">Следующие свойства также можно использовать с объектом контекста данных в шаблонах.</span><span class="sxs-lookup"><span data-stu-id="5ff48-128">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="5ff48-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ff48-129">Property</span></span> | <span data-ttu-id="5ff48-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5ff48-130">Description</span></span>                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5ff48-131">$index</span><span class="sxs-lookup"><span data-stu-id="5ff48-131">$index</span></span>   | <span data-ttu-id="5ff48-132">Числовая индексация элемента, отрисовываемого при циклической отрисовки. `data-for`</span><span class="sxs-lookup"><span data-stu-id="5ff48-132">Numerical index of item being rendered while being looped with `data-for`.</span></span>                                     |
| <span data-ttu-id="5ff48-133">$parent</span><span class="sxs-lookup"><span data-stu-id="5ff48-133">$parent</span></span>  | <span data-ttu-id="5ff48-134">Если шаблон отрисовки в другом шаблоне, это свойство позволяет получить доступ к контексту родительских данных.</span><span class="sxs-lookup"><span data-stu-id="5ff48-134">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="5ff48-135">В следующем примере показано, как `$index` использовать свойство в цикле для данных.</span><span class="sxs-lookup"><span data-stu-id="5ff48-135">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

## <a name="conditional-rendering"></a><span data-ttu-id="5ff48-136">Условная отрисовка</span><span class="sxs-lookup"><span data-stu-id="5ff48-136">Conditional rendering</span></span>

<span data-ttu-id="5ff48-137">Отрисовка элементов может потребоваться только в том случае, если условие имеет истинное или ложное на основе контекста данных.</span><span class="sxs-lookup"><span data-stu-id="5ff48-137">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="5ff48-138">Атрибуты `data-if` и выражения могут оцениваться и отрисовки, `data-else` только если засвеяется true или false.</span><span class="sxs-lookup"><span data-stu-id="5ff48-138">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="5ff48-139">Циклы</span><span class="sxs-lookup"><span data-stu-id="5ff48-139">Looping</span></span>

<span data-ttu-id="5ff48-140">В некоторых случаях объект контекста данных содержит цикл, и вам потребуется зациклить данные.</span><span class="sxs-lookup"><span data-stu-id="5ff48-140">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="5ff48-141">В этом сценарии используйте `data-for` атрибут.</span><span class="sxs-lookup"><span data-stu-id="5ff48-141">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a><span data-ttu-id="5ff48-142">Контекст шаблона</span><span class="sxs-lookup"><span data-stu-id="5ff48-142">Template context</span></span>

<span data-ttu-id="5ff48-143">В сценариях, где необходимо преобразовывать данные в привязках, привязывать к событиям или просто использовать внешние данные в привязках шаблонов, шаблоны поддерживают привязку к контексту внешних данных.</span><span class="sxs-lookup"><span data-stu-id="5ff48-143">In scenarios where you need to convert data in your bindings, bind to events, or just use external data in your templates bindings, the templates support binding to external data context.</span></span> <span data-ttu-id="5ff48-144">Добавить дополнительный контекст шаблона можно двумя способами:</span><span class="sxs-lookup"><span data-stu-id="5ff48-144">You can add additional template context in two ways:</span></span>

1. <span data-ttu-id="5ff48-145">Непосредственно на компоненте.</span><span class="sxs-lookup"><span data-stu-id="5ff48-145">Directly on the component.</span></span>

    <span data-ttu-id="5ff48-146">Каждый компонент определяет свойство, которое можно использовать для передачи дополнительных данных любому `templateContext` шаблону в компоненте.</span><span class="sxs-lookup"><span data-stu-id="5ff48-146">Each component defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span>

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    <span data-ttu-id="5ff48-147">Теперь свойства в объекте будут доступны для использования в выражениях привязки `templateContext` в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="5ff48-147">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

2. <span data-ttu-id="5ff48-148">Глобально для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="5ff48-148">Globally for all components.</span></span>

    <span data-ttu-id="5ff48-149">Класс предоставляет объект для добавления данных или функций, которые должны быть глобально `TemplateHelper` `globalContext` доступны для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="5ff48-149">The `TemplateHelper` class exposes the `globalContext` object to add data or functions that should be globally available for all components.</span></span>

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a><span data-ttu-id="5ff48-150">Конвертеры</span><span class="sxs-lookup"><span data-stu-id="5ff48-150">Converters</span></span>

<span data-ttu-id="5ff48-151">Во многих случаях может потребоваться преобразовать данные, прежде чем их представить в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="5ff48-151">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="5ff48-152">Например, может потребоваться правильно отформаировать дату перед ее отрисовка.</span><span class="sxs-lookup"><span data-stu-id="5ff48-152">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="5ff48-153">В таких случаях может потребоваться использовать конвертер шаблонов.</span><span class="sxs-lookup"><span data-stu-id="5ff48-153">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="5ff48-154">Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет делать преобразование.</span><span class="sxs-lookup"><span data-stu-id="5ff48-154">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="5ff48-155">Например, можно определить функцию для преобразования объекта события в форматированный диапазон времени.</span><span class="sxs-lookup"><span data-stu-id="5ff48-155">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="5ff48-156">Чтобы использовать преобразователь в шаблоне, используйте его так, как если бы вы использовали функцию в коде кода.</span><span class="sxs-lookup"><span data-stu-id="5ff48-156">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="5ff48-157">Привязка события или свойства</span><span class="sxs-lookup"><span data-stu-id="5ff48-157">Event or property binding</span></span>

<span data-ttu-id="5ff48-158">Этот атрибут позволяет добавить прослушиватель событий или установить значение `data-props` свойства непосредственно в шаблонах.</span><span class="sxs-lookup"><span data-stu-id="5ff48-158">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span>

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="5ff48-159">Реквизиты данных принимают строку с запятой для каждого свойства или обработника событий, которые вы можете захотим установить.</span><span class="sxs-lookup"><span data-stu-id="5ff48-159">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span>

<span data-ttu-id="5ff48-160">Чтобы добавить обработтель событий, добавьте к имени события префикс `@` .</span><span class="sxs-lookup"><span data-stu-id="5ff48-160">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="5ff48-161">Обработник событий должен быть доступен в `templateContext` элементе.</span><span class="sxs-lookup"><span data-stu-id="5ff48-161">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="5ff48-162">Args события, контекст данных и корневой элемент шаблона передаются обработчиве событий в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="5ff48-162">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="5ff48-163">Событие отображения шаблона</span><span class="sxs-lookup"><span data-stu-id="5ff48-163">Template rendered event</span></span>

<span data-ttu-id="5ff48-164">В некоторых случаях может потребоваться получить ссылку на элемент отрисовки.</span><span class="sxs-lookup"><span data-stu-id="5ff48-164">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="5ff48-165">Это может быть полезно, если вы хотите самостоятельно обрабатывать отрисовку содержимого или хотите изменить элемент отрисовки.</span><span class="sxs-lookup"><span data-stu-id="5ff48-165">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="5ff48-166">В этом сценарии можно использовать событие, которое сгореет после отрисовки `templateRendered` шаблона.</span><span class="sxs-lookup"><span data-stu-id="5ff48-166">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="5ff48-167">Сведения о событии будут содержать ссылку на элемент, который отрисовки, объект контекста данных и тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="5ff48-167">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="5ff48-168">Стиль</span><span class="sxs-lookup"><span data-stu-id="5ff48-168">Styling</span></span>

<span data-ttu-id="5ff48-169">Шаблоны можно стиль обычно с помощью CSS, так как они отрисовки за пределами теневой dom.</span><span class="sxs-lookup"><span data-stu-id="5ff48-169">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
