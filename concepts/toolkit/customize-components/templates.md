---
title: Шаблоны в microsoft Graph набор средств
description: Используйте настраиваемые шаблоны для изменения контента компонента.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 1db3f315cd89932481a0a2325eecae19592d9276
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963283"
---
# <a name="templates-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="62ad8-103">Шаблоны в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="62ad8-103">Templates in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="62ad8-104">Большинство компонентов Microsoft Graph набор средств поддерживают использование настраиваемого шаблона для изменения содержимого компонента.</span><span class="sxs-lookup"><span data-stu-id="62ad8-104">Most Microsoft Graph Toolkit components support the use of custom templates to modify the content of a component.</span></span>

<span data-ttu-id="62ad8-105">Все веб-компоненты поддерживают шаблоны на основе `<template>` элемента.</span><span class="sxs-lookup"><span data-stu-id="62ad8-105">All web components support templates based on the `<template>` element.</span></span> <span data-ttu-id="62ad8-106">Например, чтобы переопредить шаблон компонента, добавьте элемент `<template>` внутри компонента.</span><span class="sxs-lookup"><span data-stu-id="62ad8-106">For example, to override the template of a component, add a `<template>` element inside a component.</span></span>

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

<span data-ttu-id="62ad8-107">Если вы используете компоненты Microsoft Graph набор средств React, вы можете использовать React для оформления шаблонов.</span><span class="sxs-lookup"><span data-stu-id="62ad8-107">If you're using the Microsoft Graph Toolkit React components, you can use React for authoring templates.</span></span> <span data-ttu-id="62ad8-108">Подробные сведения [см. в материале Use the toolkit with React.](../get-started/mgt-react.md)</span><span class="sxs-lookup"><span data-stu-id="62ad8-108">For details, see [Use the toolkit with React](../get-started/mgt-react.md).</span></span>

## <a name="data-type"></a><span data-ttu-id="62ad8-109">Тип данных</span><span class="sxs-lookup"><span data-stu-id="62ad8-109">Data-type</span></span>

<span data-ttu-id="62ad8-110">Каждый компонент может иметь несколько частей, которые можно шаблонить.</span><span class="sxs-lookup"><span data-stu-id="62ad8-110">Each component can have multiple parts that can be templated.</span></span> <span data-ttu-id="62ad8-111">Например, в компоненте можно шаблонить отдельные события, отдельные заглавные разделы, представление загрузки, отсутствие представления `mgt-agenda` данных и т. д.</span><span class="sxs-lookup"><span data-stu-id="62ad8-111">For example, in the `mgt-agenda` component, you can template individual events, individual section headers, loading view, no data view, and more.</span></span> <span data-ttu-id="62ad8-112">Чтобы указать шаблон, используйте `data-type` атрибут в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="62ad8-112">To indicate the template, use the `data-type` attribute on a template.</span></span> <span data-ttu-id="62ad8-113">Например, для шаблона каждого события `mgt-agenda` в , используйте тип `event` данных, как показано.</span><span class="sxs-lookup"><span data-stu-id="62ad8-113">For example, to template each event in the `mgt-agenda`, use the `event` data-type, as shown.</span></span>

```html
<mgt-agenda>
  <template data-type="event"> </template>
</mgt-agenda>
```

<span data-ttu-id="62ad8-114">Если `data-type` нет, весь компонент будет заменен шаблоном.</span><span class="sxs-lookup"><span data-stu-id="62ad8-114">If no `data-type` is specified, the entire component will be replaced with the template.</span></span> <span data-ttu-id="62ad8-115">Вы также можете использовать `data-type="default"` для той же цели.</span><span class="sxs-lookup"><span data-stu-id="62ad8-115">You can also use `data-type="default"` for the same purpose.</span></span>

## <a name="binding-data"></a><span data-ttu-id="62ad8-116">Привязка данных</span><span class="sxs-lookup"><span data-stu-id="62ad8-116">Binding data</span></span>

<span data-ttu-id="62ad8-117">Многие шаблоны позволяют связывать данные, которые передаются в шаблон в качестве контекста данных.</span><span class="sxs-lookup"><span data-stu-id="62ad8-117">Many templates allow binding of data that is passed to the template as data context.</span></span> <span data-ttu-id="62ad8-118">Например, шаблон в компоненте передает объект, который можно `event` `mgt-agenda` использовать непосредственно в `{event}` шаблоне.</span><span class="sxs-lookup"><span data-stu-id="62ad8-118">For example, the `event` template in the `mgt-agenda` component passes an `{event}` object that can be used directly in the template.</span></span> <span data-ttu-id="62ad8-119">Чтобы расширить выражение, `event.subject` например, используйте двойные фигурные скобки.</span><span class="sxs-lookup"><span data-stu-id="62ad8-119">To expand an expression, such as `event.subject`, use the double curly brackets.</span></span>

```html
<template data-type="event">
  <div>{{event.subject}}</div>
</template>
```

<span data-ttu-id="62ad8-120">Этот формат также можно использовать в атрибутах:</span><span class="sxs-lookup"><span data-stu-id="62ad8-120">This format can also be used inside attributes:</span></span>

```html
<template data-type="event">
  <a href="{{ event.onlineMeetingUrl }}" />
</template>
```

> <span data-ttu-id="62ad8-121">**Примечание:** Вы также можете расширить объекты, такие как или и они `{{event}}` `{{this}}` будут отрисовки в качестве строк JSON.</span><span class="sxs-lookup"><span data-stu-id="62ad8-121">**Note:** You can also expand objects such as `{{event}}` or `{{this}}` and they will render as JSON strings.</span></span> <span data-ttu-id="62ad8-122">Это может быть полезно при разработке шаблонов.</span><span class="sxs-lookup"><span data-stu-id="62ad8-122">This can be useful when you're developing the templates.</span></span>

### <a name="change-binding-syntax"></a><span data-ttu-id="62ad8-123">Изменение синтаксиса привязки</span><span class="sxs-lookup"><span data-stu-id="62ad8-123">Change binding syntax</span></span>

<span data-ttu-id="62ad8-124">По умолчанию для расширения выражения используются двойные фигурные скобки ( `{{expression}}` ).</span><span class="sxs-lookup"><span data-stu-id="62ad8-124">By default, to expand an expression, you use double curly brackets ( `{{expression}}` ).</span></span> <span data-ttu-id="62ad8-125">Однако этот синтаксис можно изменить для сред, в которых уже используется синтаксис двойной фигурной скобки.</span><span class="sxs-lookup"><span data-stu-id="62ad8-125">However, you can change this syntax for environments where the double curly bracket syntax is already used.</span></span> <span data-ttu-id="62ad8-126">Например, в следующем примере используются двойные квадратные скобки ( `[[expression]]` ).</span><span class="sxs-lookup"><span data-stu-id="62ad8-126">For example, the following example uses double square brackets ( `[[expression]]` ).</span></span>

```ts
import { TemplateHelper } from '@microsoft/mgt';

TemplateHelper.setBindingSyntax('[[', ']]');
```

## <a name="data-context-helper-properties"></a><span data-ttu-id="62ad8-127">Свойства помощника контекста данных</span><span class="sxs-lookup"><span data-stu-id="62ad8-127">Data context helper properties</span></span>

<span data-ttu-id="62ad8-128">Следующие свойства также можно использовать с объектом контекста данных в шаблонах.</span><span class="sxs-lookup"><span data-stu-id="62ad8-128">The following properties can also be used with the data context object in your templates.</span></span>

| <span data-ttu-id="62ad8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="62ad8-129">Property</span></span> | <span data-ttu-id="62ad8-130">Описание</span><span class="sxs-lookup"><span data-stu-id="62ad8-130">Description</span></span>                                                                                                    |
|----------|----------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="62ad8-131">$index</span><span class="sxs-lookup"><span data-stu-id="62ad8-131">$index</span></span>   | <span data-ttu-id="62ad8-132">Числовая индексация элемента, отрисовываемого при цикле `data-for` с .</span><span class="sxs-lookup"><span data-stu-id="62ad8-132">Numerical index of item being rendered while being looped with `data-for`.</span></span>                                     |
| <span data-ttu-id="62ad8-133">$parent</span><span class="sxs-lookup"><span data-stu-id="62ad8-133">$parent</span></span>  | <span data-ttu-id="62ad8-134">Если шаблон отрисовка внутри другого шаблона, это свойство позволяет получить доступ к родительскому контексту данных.</span><span class="sxs-lookup"><span data-stu-id="62ad8-134">If a template is rendered inside another template, this property allows you to access the parent data context.</span></span> |

<span data-ttu-id="62ad8-135">В следующем примере показано, как использовать `$index` свойство в цикле data-for.</span><span class="sxs-lookup"><span data-stu-id="62ad8-135">The following example shows how to use the `$index` property in a data-for loop.</span></span>

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

### <a name="this"></a><span data-ttu-id="62ad8-136">{{this}}</span><span class="sxs-lookup"><span data-stu-id="62ad8-136">{{this}}</span></span>

<span data-ttu-id="62ad8-137">Чтобы помочь отламыть контекст данных, можно использовать в `this` выражениях привязки.</span><span class="sxs-lookup"><span data-stu-id="62ad8-137">To help debug the data context, you can use `this` in your binding expressions.</span></span> <span data-ttu-id="62ad8-138">Простейшая форма заключается в добавлении `{{this}}` в любом месте шаблона.</span><span class="sxs-lookup"><span data-stu-id="62ad8-138">The simplest form is to add `{{this}}` anywhere in your template.</span></span>

```html
<template data-type="event">
  <div>
    {{this}}
  </div>
</template>
```

<span data-ttu-id="62ad8-139">Так как JavaScript можно использовать в выражениях привязки, у вас также есть доступ к объекту, который позволяет использовать (или любой другой [`console`](https://developer.mozilla.org/docs/Web/API/Console) `console.log(this)` API) в `console` шаблонах.</span><span class="sxs-lookup"><span data-stu-id="62ad8-139">Because you can use JavaScript in your binding expressions, you also have access to the [`console`](https://developer.mozilla.org/docs/Web/API/Console) object which allows you to use `console.log(this)` (or any other `console` API) in your templates.</span></span>

```html
<template data-type="event">
  <div>
    {{console.log(this)}}
  </div>
</template>
```

## <a name="conditional-rendering"></a><span data-ttu-id="62ad8-140">Условное отрисовка</span><span class="sxs-lookup"><span data-stu-id="62ad8-140">Conditional rendering</span></span>

<span data-ttu-id="62ad8-141">Отрисовка элементов может потребоваться только в том случае, если условие является верным или ложным на основе контекста данных.</span><span class="sxs-lookup"><span data-stu-id="62ad8-141">You might only want to render elements when a condition is true or false based on the data context.</span></span> <span data-ttu-id="62ad8-142">Атрибуты `data-if` `data-else` и выражения могут оцениваться и отрисовки только в том случае, если они верны или ложны.</span><span class="sxs-lookup"><span data-stu-id="62ad8-142">The `data-if` and `data-else` attributes can evaluate an expression and render only if true or false.</span></span>

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

## <a name="looping"></a><span data-ttu-id="62ad8-143">Цикл</span><span class="sxs-lookup"><span data-stu-id="62ad8-143">Looping</span></span>

<span data-ttu-id="62ad8-144">Будут случаи, когда объект контекста данных содержит цикл, и вам потребуется цикл данных.</span><span class="sxs-lookup"><span data-stu-id="62ad8-144">There will be cases where the data context object contains loop and you will need to loop over the data.</span></span> <span data-ttu-id="62ad8-145">Для этого сценария используйте `data-for` атрибут.</span><span class="sxs-lookup"><span data-stu-id="62ad8-145">For this scenario, use the `data-for` attribute.</span></span>

```html
<template data-type="event">
  <ul>
    <li data-for='attendee in event.attendees'>
      {{ attendee.displayName }}
    </li>
  </ul>
</template>
```

## <a name="template-context"></a><span data-ttu-id="62ad8-146">Контекст шаблона</span><span class="sxs-lookup"><span data-stu-id="62ad8-146">Template context</span></span>

<span data-ttu-id="62ad8-147">В сценариях, в которых необходимо преобразовать данные в привязки, привязать к событиям или просто использовать внешние данные в привязках шаблонов, шаблоны поддерживают привязку к внешнему контексту данных.</span><span class="sxs-lookup"><span data-stu-id="62ad8-147">In scenarios where you need to convert data in your bindings, bind to events, or just use external data in your templates bindings, the templates support binding to external data context.</span></span> <span data-ttu-id="62ad8-148">Дополнительный контекст шаблона можно добавить двумя способами:</span><span class="sxs-lookup"><span data-stu-id="62ad8-148">You can add additional template context in two ways:</span></span>

1. <span data-ttu-id="62ad8-149">Непосредственно на компоненте.</span><span class="sxs-lookup"><span data-stu-id="62ad8-149">Directly on the component.</span></span>

    <span data-ttu-id="62ad8-150">Каждый компонент определяет свойство, которое можно использовать для передачи дополнительных данных любому `templateContext` шаблону в компоненте.</span><span class="sxs-lookup"><span data-stu-id="62ad8-150">Each component defines the `templateContext` property, which you can use to pass additional data to any template in the component.</span></span>

    ```ts
    document.querySelector('mgt-agenda').templateContext = {

      someObject: {},
      formatDate: (date: Date) => { /* format date and return */ },
      someEventHandler: (e) => { /* handleEvent */  }

    }
    ```

    <span data-ttu-id="62ad8-151">Свойства объекта теперь будут доступны для использования в выражениях `templateContext` привязки в шаблоне.</span><span class="sxs-lookup"><span data-stu-id="62ad8-151">The properties in the `templateContext` object will now be available to be used in the binding expressions in the template.</span></span>

2. <span data-ttu-id="62ad8-152">Глобально для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="62ad8-152">Globally for all components.</span></span>

    <span data-ttu-id="62ad8-153">Класс предоставляет объекту возможность добавлять данные или функции, которые должны быть глобально `TemplateHelper` `globalContext` доступны для всех компонентов.</span><span class="sxs-lookup"><span data-stu-id="62ad8-153">The `TemplateHelper` class exposes the `globalContext` object to add data or functions that should be globally available for all components.</span></span>

    ```ts
    import { TemplateHelper } from '@microsoft/mgt';

    TemplateHelper.globalContext.someObject = {};
    TemplateHelper.globalContext.formatDate = (date: Date) => { /* format date and return */ };
    TemplateHelper.globalContext.someEventHandler = (e) => { /* handleEvent */  }
    ```



### <a name="converters"></a><span data-ttu-id="62ad8-154">Преобразователи</span><span class="sxs-lookup"><span data-stu-id="62ad8-154">Converters</span></span>

<span data-ttu-id="62ad8-155">Во многих случаях перед тем, как представить их в шаблоне, может потребоваться преобразовать данные.</span><span class="sxs-lookup"><span data-stu-id="62ad8-155">In many cases, you might want to transform the data before presenting it in the template.</span></span> <span data-ttu-id="62ad8-156">Например, перед отрисовки может потребоваться правильное форматирование даты.</span><span class="sxs-lookup"><span data-stu-id="62ad8-156">For example, you might want to properly format a date before it is rendered.</span></span> <span data-ttu-id="62ad8-157">В этих случаях может потребоваться использовать конвертер шаблонов.</span><span class="sxs-lookup"><span data-stu-id="62ad8-157">In these cases, you might want to use a template converter.</span></span>

<span data-ttu-id="62ad8-158">Чтобы использовать конвертер шаблонов, сначала необходимо определить функцию, которая будет делать преобразование.</span><span class="sxs-lookup"><span data-stu-id="62ad8-158">To use a template converter, you first need to define a function that will do the conversion.</span></span> <span data-ttu-id="62ad8-159">Например, можно определить функцию преобразования объекта события в отформатированный диапазон времени.</span><span class="sxs-lookup"><span data-stu-id="62ad8-159">For example, you might define a function to convert an event object to a formatted time range.</span></span>

```ts
document.querySelector('mgt-agenda').templateContext = {

  getTimeRange: (event) => {
    // TODO: format a string from the event object as you wish
    // timeRange = ...

    return timeRange;
  }

}
```

<span data-ttu-id="62ad8-160">Чтобы использовать конвертер в шаблоне, используйте его так, как если бы вы использовали функцию в коде позади.</span><span class="sxs-lookup"><span data-stu-id="62ad8-160">To use the converter in your template, use it as if you would use a function in code behind.</span></span>

```html
<template data-type="event">
  <div>{{ getTimeRange(event) }}</div>
</template>
```

### <a name="event-or-property-binding"></a><span data-ttu-id="62ad8-161">Привязка события или свойства</span><span class="sxs-lookup"><span data-stu-id="62ad8-161">Event or property binding</span></span>

<span data-ttu-id="62ad8-162">Атрибут позволяет добавлять слушателя событий или устанавливать значение `data-props` свойства непосредственно в шаблонах.</span><span class="sxs-lookup"><span data-stu-id="62ad8-162">The `data-props` attribute allows you to add an event listener or set a property value directly in your templates.</span></span>

```html
<template>
    <button data-props="{{@click: myEvent, myProp: value}}"></button>
</template>
```

<span data-ttu-id="62ad8-163">Реквизит данных принимает запятую, делимитированную строку для каждого свойства или обработника событий, которые может потребоваться установить.</span><span class="sxs-lookup"><span data-stu-id="62ad8-163">The data-props accepts a comma delimited string for each property or event handler you might want to set.</span></span>

<span data-ttu-id="62ad8-164">Чтобы добавить обработник событий, пристройте имя события с `@` помощью .</span><span class="sxs-lookup"><span data-stu-id="62ad8-164">To add an event handler, prefix the name of the event with `@`.</span></span> <span data-ttu-id="62ad8-165">Обработник событий должен быть доступен в `templateContext` элементе.</span><span class="sxs-lookup"><span data-stu-id="62ad8-165">The event handler will need to be available in the `templateContext` of the element.</span></span>

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

<span data-ttu-id="62ad8-166">Args события, контекст данных и корневой элемент шаблона передаются обработчиве событий в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="62ad8-166">The event args, data context, and the root element of the template are passed to the event handler as parameters.</span></span>


## <a name="template-rendered-event"></a><span data-ttu-id="62ad8-167">Событие отрисовки шаблона</span><span class="sxs-lookup"><span data-stu-id="62ad8-167">Template rendered event</span></span>

<span data-ttu-id="62ad8-168">В некоторых случаях может потребоваться получить ссылку на отрисовка элемента.</span><span class="sxs-lookup"><span data-stu-id="62ad8-168">In certain cases, you might want to get a reference to the rendered element.</span></span> <span data-ttu-id="62ad8-169">Это может быть полезно, если вы хотите самостоятельно обрабатывать отрисовку контента или изменить отрисовку элемента.</span><span class="sxs-lookup"><span data-stu-id="62ad8-169">This can be useful if you want to handle the rendering of the content yourself, or you want to modify the rendered element.</span></span>

<span data-ttu-id="62ad8-170">В этом сценарии можно использовать событие, которое загорелось после отрисовки `templateRendered` шаблона.</span><span class="sxs-lookup"><span data-stu-id="62ad8-170">In this scenario, you can use the `templateRendered` event, which fires after the template has been rendered.</span></span>

```ts
let agenda = document.querySelector('mgt-agenda');
agenda.addEventListener('templateRendered', (e) => { });
```

<span data-ttu-id="62ad8-171">Сведения о событии будут содержать ссылку на отрисовка элемента, объект контекста данных и тип шаблона.</span><span class="sxs-lookup"><span data-stu-id="62ad8-171">The event details will contain a reference to the element that is being rendered, the data context object, and the type of the template.</span></span>

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

## <a name="styling"></a><span data-ttu-id="62ad8-172">Стиль</span><span class="sxs-lookup"><span data-stu-id="62ad8-172">Styling</span></span>

<span data-ttu-id="62ad8-173">Шаблоны можно в обычном режиме стилизовать с помощью CSS, так как они отрисовыются за пределами теневого дома.</span><span class="sxs-lookup"><span data-stu-id="62ad8-173">The templates can be styled normally via CSS as they are rendered outside of the shadow dom.</span></span>
