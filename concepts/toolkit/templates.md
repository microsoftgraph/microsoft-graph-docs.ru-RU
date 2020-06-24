---
title: Шаблоны в наборе инструментов Microsoft Graph
description: Используйте настраиваемые шаблоны для изменения содержимого компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 4f855558b8b1ee5d0f84b9998b62c2f770a4dc6b
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845955"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="aa701-103">Шаблоны в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aa701-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="aa701-104">Используйте настраиваемые шаблоны для изменения содержимого компонента.</span><span class="sxs-lookup"><span data-stu-id="aa701-104">Use custom templates to modify the content of a component.</span></span>

<span data-ttu-id="aa701-105">Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента.</span><span class="sxs-lookup"><span data-stu-id="aa701-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="aa701-106">Например, чтобы переопределить шаблон компонента, добавьте `<template>` элемент в компонент.</span><span class="sxs-lookup"><span data-stu-id="aa701-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

## <a name="data-type"></a><span data-ttu-id="aa701-107">Тип данных</span><span class="sxs-lookup"><span data-stu-id="aa701-107">Data-type</span></span>

<span data-ttu-id="aa701-108">Каждый компонент может иметь несколько частей, которые можно использовать в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="aa701-108">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="aa701-109">Например, в `mgt-agenda` компоненте можно зашаблонировать отдельные события, заголовки отдельных разделов, Загрузка представления, без представления данных и т. д.</span><span class="sxs-lookup"><span data-stu-id="aa701-109">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="aa701-110">Чтобы указать шаблон, используйте `data-type` атрибут для шаблона.</span><span class="sxs-lookup"><span data-stu-id="aa701-110">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="aa701-111">Например, чтобы указать шаблон для каждого события в `mgt-agenda` , используйте `event` тип данных, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="aa701-111">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="aa701-112">Если этот параметр не `data-type` указан, весь компонент будет заменен на шаблон.</span><span class="sxs-lookup"><span data-stu-id="aa701-112">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="aa701-113">Вы также можете использовать `data-type="default"` для этой цели.</span><span class="sxs-lookup"><span data-stu-id="aa701-113">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="aa701-114">Привязка данных</span><span class="sxs-lookup"><span data-stu-id="aa701-114">Binding data</span></span>

<span data-ttu-id="aa701-115">Многие шаблоны позволяют привязать данные, которые передаются шаблону в качестве контекста данных.</span><span class="sxs-lookup"><span data-stu-id="aa701-115">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="aa701-116">Например, `event` шаблон в `mgt-agenda` компоненте передает `{event}` объект, который можно использовать непосредственно в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="aa701-116">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="aa701-117">Чтобы развернуть выражение, например `event.subject` , используйте двойные фигурные скобки.</span><span class="sxs-lookup"><span data-stu-id="aa701-117">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="aa701-118">Этот формат также можно использовать внутри атрибутов:</span><span class="sxs-lookup"><span data-stu-id="aa701-118">This format can also be used inside attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="aa701-119">**Примечание:** Вы также можете развернуть такие объекты, как `{{event}}` , и они будут отображаться как строки JSON.</span><span class="sxs-lookup"><span data-stu-id="aa701-119">**Note:** You can also expand objects such as `{{event}}` and they will render as JSON strings.</span></span> <span data-ttu-id="aa701-120">Это может быть удобно при разработке шаблонов.</span><span class="sxs-lookup"><span data-stu-id="aa701-120">This can be useful when you're developing the templates.</span></span>

### <a name="change-binding-syntax"></a><span data-ttu-id="aa701-121">Изменение синтаксиса привязки</span><span class="sxs-lookup"><span data-stu-id="aa701-121">Change binding syntax</span></span>

<span data-ttu-id="aa701-122">По умолчанию для расширения выражения используются двойные фигурные скобки ( `{{expression}}` ).</span><span class="sxs-lookup"><span data-stu-id="aa701-122">By default, to expand an expression, you use double curly brackets ( `{{expression}}` ).</span></span> <span data-ttu-id="aa701-123">Однако этот синтаксис можно изменить для сред, в которых уже используется синтаксис двойной фигурной скобки.</span><span class="sxs-lookup"><span data-stu-id="aa701-123">However, you can change this syntax for environments where the double curly bracket syntax is already used.</span></span> <span data-ttu-id="aa701-124">Например, в приведенном ниже примере используются двойные квадратные скобки ( `[[expression]]` ).</span><span class="sxs-lookup"><span data-stu-id="aa701-124">For example, the following example uses double square brackets ( `[[expression]]` ).</span></span>

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a><span data-ttu-id="aa701-125">Вспомогательные свойства контекста данных</span><span class="sxs-lookup"><span data-stu-id="aa701-125">Data context helper properties</span></span>

<span data-ttu-id="aa701-126">Следующие свойства также можно использовать с объектом контекста данных в шаблонах.</span><span class="sxs-lookup"><span data-stu-id="aa701-126">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="aa701-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa701-127">Property</span></span> | <span data-ttu-id="aa701-128">Описание</span><span class="sxs-lookup"><span data-stu-id="aa701-128">Description</span></span>                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="aa701-129">$index</span><span class="sxs-lookup"><span data-stu-id="aa701-129">$index</span></span>   | <span data-ttu-id="aa701-130">Числовой индекс элемента, отображаемого в цикле `data-for` .</span><span class="sxs-lookup"><span data-stu-id="aa701-130">Numerical index of item being rendered while being looped with `data-for`.</span></span>                                     |
| <span data-ttu-id="aa701-131">$parent</span><span class="sxs-lookup"><span data-stu-id="aa701-131">$parent</span></span>  | <span data-ttu-id="aa701-132">Если шаблон отображается в другом шаблоне, это свойство позволяет получить доступ к родительскому контексту данных.</span><span class="sxs-lookup"><span data-stu-id="aa701-132">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="aa701-133">В приведенном ниже примере показано, как использовать `$index` свойство в цикле обработки данных.</span><span class="sxs-lookup"><span data-stu-id="aa701-133">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

## <a name="conditional-rendering"></a><span data-ttu-id="aa701-134">Условная визуализация</span><span class="sxs-lookup"><span data-stu-id="aa701-134">Conditional rendering</span></span>

<span data-ttu-id="aa701-135">Вы можете отображать элементы только в том случае, если условие имеет значение true или false в зависимости от контекста данных.</span><span class="sxs-lookup"><span data-stu-id="aa701-135">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="aa701-136">`data-if`Атрибуты и `data-else` могут оценивать выражение и отображать только значения true и false.</span><span class="sxs-lookup"><span data-stu-id="aa701-136">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="aa701-137">Циклов</span><span class="sxs-lookup"><span data-stu-id="aa701-137">Looping</span></span>

<span data-ttu-id="aa701-138">Существуют случаи, когда объект контекста данных содержит цикл, и вам потребуется перебрать данные.</span><span class="sxs-lookup"><span data-stu-id="aa701-138">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="aa701-139">В этом случае используйте `data-for` атрибут.</span><span class="sxs-lookup"><span data-stu-id="aa701-139">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a><span data-ttu-id="aa701-140">Контекст шаблона</span><span class="sxs-lookup"><span data-stu-id="aa701-140">Template context</span></span>

<span data-ttu-id="aa701-141">В сценариях, в которых необходимо преобразовать данные в привязке, выполнить привязку к событиям или просто использовать внешние данные в привязках шаблонов, шаблоны поддерживают привязку к внешнему содержимому данных.</span><span class="sxs-lookup"><span data-stu-id="aa701-141">In scenarios where you need to convert data in your bindings, bind to events, or just use external data in your templates bindings, the templates support binding to external data context.</span></span> <span data-ttu-id="aa701-142">Вы можете добавить дополнительный контекст шаблона двумя способами:</span><span class="sxs-lookup"><span data-stu-id="aa701-142">You can add additional template context in two ways:</span></span>

1. <span data-ttu-id="aa701-143">Непосредственно на компоненте.</span><span class="sxs-lookup"><span data-stu-id="aa701-143">Directly on the component.</span></span>

    <span data-ttu-id="aa701-144">Каждый компонент определяет `templateContext` свойство, которое можно использовать для передачи дополнительных данных любому шаблону в компоненте.</span><span class="sxs-lookup"><span data-stu-id="aa701-144">Each component defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span>

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    <span data-ttu-id="aa701-145">Теперь свойства объекта станут `templateContext` доступны для использования в выражениях привязки в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="aa701-145">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

2. <span data-ttu-id="aa701-146">Глобально для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="aa701-146">Globally for all components.</span></span>

    <span data-ttu-id="aa701-147">`TemplateHelper`Класс предоставляет `globalContext` объект для добавления данных или функций, которые должны быть глобально доступными для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="aa701-147">The `TemplateHelper` class exposes the `globalContext` object to add data or functions that should be globally available for all components.</span></span>

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a><span data-ttu-id="aa701-148">Типов</span><span class="sxs-lookup"><span data-stu-id="aa701-148">Converters</span></span>

<span data-ttu-id="aa701-149">Во многих случаях может потребоваться преобразовать данные перед их представлением в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="aa701-149">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="aa701-150">Например, вам может потребоваться правильно отформатировать дату перед отображением.</span><span class="sxs-lookup"><span data-stu-id="aa701-150">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="aa701-151">В таких случаях может потребоваться использование конвертера шаблонов.</span><span class="sxs-lookup"><span data-stu-id="aa701-151">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="aa701-152">Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет выполнять преобразование.</span><span class="sxs-lookup"><span data-stu-id="aa701-152">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="aa701-153">Например, вы можете определить функцию для преобразования объекта события в отформатированный диапазон времени.</span><span class="sxs-lookup"><span data-stu-id="aa701-153">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="aa701-154">Чтобы использовать конвертер в шаблоне, используйте его, как если бы вы использовали функцию в коде программной части.</span><span class="sxs-lookup"><span data-stu-id="aa701-154">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="aa701-155">Привязка события или свойства</span><span class="sxs-lookup"><span data-stu-id="aa701-155">Event or property binding</span></span>

<span data-ttu-id="aa701-156">`data-props`Атрибут позволяет добавить прослушиватель событий или задать значение свойства непосредственно в шаблонах.</span><span class="sxs-lookup"><span data-stu-id="aa701-156">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span>

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="aa701-157">Свойства Data/PROPS принимают строку с разделителями запятыми для каждого свойства или обработчика событий, который может потребоваться задать.</span><span class="sxs-lookup"><span data-stu-id="aa701-157">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span>

<span data-ttu-id="aa701-158">Чтобы добавить обработчик событий, добавьте к имени события префикс `@` .</span><span class="sxs-lookup"><span data-stu-id="aa701-158">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="aa701-159">Обработчик события должен быть доступен в `templateContext` элементе.</span><span class="sxs-lookup"><span data-stu-id="aa701-159">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="aa701-160">Аргументы события, контекст данных и корневой элемент шаблона передаются обработчику событий в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="aa701-160">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="aa701-161">Событие, отображаемое в шаблоне</span><span class="sxs-lookup"><span data-stu-id="aa701-161">Template rendered event</span></span>

<span data-ttu-id="aa701-162">В некоторых случаях может потребоваться получить ссылку на визуализированный элемент.</span><span class="sxs-lookup"><span data-stu-id="aa701-162">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="aa701-163">Это может быть удобно, если вы хотите самостоятельно обработать отображение контента или изменить отображаемый элемент.</span><span class="sxs-lookup"><span data-stu-id="aa701-163">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="aa701-164">В этом сценарии можно использовать `templateRendered` событие, которое срабатывает после отображения шаблона.</span><span class="sxs-lookup"><span data-stu-id="aa701-164">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="aa701-165">Сведения о событии будут содержать ссылку на отображаемый элемент, объект контекста данных и тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="aa701-165">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="aa701-166">Изменении</span><span class="sxs-lookup"><span data-stu-id="aa701-166">Styling</span></span>

<span data-ttu-id="aa701-167">Шаблоны можно обычно отформатировать с помощью CSS, так как они отображаются вне теневой модели DOM.</span><span class="sxs-lookup"><span data-stu-id="aa701-167">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
