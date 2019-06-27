---
title: Компонент повестки в наборе инструментов Microsoft Graph
description: Веб-компонент "центр центровой связи" используется для представления событий в календаре пользователя или группы.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 8a91b20a48c1646fafd8cd7a287f037615024a73
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243086"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="db179-103">Компонент повестки в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="db179-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="db179-104">`mgt-agenda` Веб-компонент представляет события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="db179-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="db179-105">По умолчанию в календаре отображаются текущие события пользователя, вошедшего в текущий день.</span><span class="sxs-lookup"><span data-stu-id="db179-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="db179-106">Компонент также может использовать любую конечную точку, возвращающую события из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="db179-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span> 

## <a name="example"></a><span data-ttu-id="db179-107">Пример</span><span class="sxs-lookup"><span data-stu-id="db179-107">Example</span></span>

[<span data-ttu-id="db179-108">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="db179-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![центр, повестка](./images/mgt-agenda.png)

## <a name="properties"></a><span data-ttu-id="db179-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="db179-110">Properties</span></span>

<span data-ttu-id="db179-111">По умолчанию `mgt-agenda` компонент получает события от `/me/calendarview` конечной точки и отображает события за текущий день.</span><span class="sxs-lookup"><span data-stu-id="db179-111">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="db179-112">Существует несколько свойств, которые можно использовать для изменения этого поведения.</span><span class="sxs-lookup"><span data-stu-id="db179-112">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="db179-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="db179-113">Property</span></span> | <span data-ttu-id="db179-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="db179-114">Attribute</span></span> | <span data-ttu-id="db179-115">Описание</span><span class="sxs-lookup"><span data-stu-id="db179-115">Description</span></span> |
| --- | --- | --- |
| `groupByDay` | `group-by-day` | <span data-ttu-id="db179-116">Логическое значение для группировки событий по дням события по умолчанию не группируются.</span><span class="sxs-lookup"><span data-stu-id="db179-116">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| `date` | `date` | <span data-ttu-id="db179-117">Строка, представляющая дату начала событий, которые необходимо получить из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="db179-117">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="db179-118">Значение должно быть в формате, который может быть проанализирован с помощью [конструктора Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -value, если `event-query` задан атрибут.</span><span class="sxs-lookup"><span data-stu-id="db179-118">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| `days` | `days` | <span data-ttu-id="db179-119">Число дней для выборки из Microsoft Graph — значение по умолчанию не оказывает никакого действия, если `event-query` задан атрибут.</span><span class="sxs-lookup"><span data-stu-id="db179-119">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| `eventQuery` | `event-query` | <span data-ttu-id="db179-120">Строка, представляющая альтернативный запрос, который будет использоваться при получении событий из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="db179-120">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="db179-121">При необходимости добавьте делегированную область в конец строки, чтобы она была ограничена `|` (`"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`).</span><span class="sxs-lookup"><span data-stu-id="db179-121">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`).</span></span> |
| `events` | `events` | <span data-ttu-id="db179-122">Массив событий, чтобы получить или задать список событий, отображаемых компонентом, с помощью этого свойства можно получить доступ к событиям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="db179-122">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="db179-123">Присвойте этому значению значение загрузка собственных событий, если значение задано разработчиком, `date`атрибуты `days`, или `event-query` , атрибуты, не действуют.</span><span class="sxs-lookup"><span data-stu-id="db179-123">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |

<span data-ttu-id="db179-124">В следующем примере показано, как изменить поведение компонента для извлечения данных за определенную дату и до 3 дней.</span><span class="sxs-lookup"><span data-stu-id="db179-124">The following example changes the behavior of the component to fetch data for a specific date and up to 3 days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="db179-125">В следующем примере показано изменение поведения компонента для извлечения данных из определенного запроса.</span><span class="sxs-lookup"><span data-stu-id="db179-125">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="db179-126">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="db179-126">CSS Custom properties</span></span>

<span data-ttu-id="db179-127">`mgt-agenda` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS</span><span class="sxs-lookup"><span data-stu-id="db179-127">The `mgt-agenda` component defines these CSS custom properties</span></span>

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background: #ffffff;
  --event-border: solid 2px rgba(0, 0, 0, 0);

  --agenda-header-margin: 40px 10px 14px 10px;
  --agenda-header-font-size: 24px;
  --agenda-header-color: #333333;

  --event-time-font-size: 12px;
  --event-time-color: #000000;

  --event-subject-font-size: 19px;
  --event-subject-color: #333333;

  --event-location-font-size: 12px;
  --event-location-color: #000000;
}
```

<span data-ttu-id="db179-128">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="db179-128">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="db179-129">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="db179-129">Templates</span></span>

<span data-ttu-id="db179-130">`mgt-agenda` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="db179-130">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="db179-131">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="db179-131">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="db179-132">Тип данных</span><span class="sxs-lookup"><span data-stu-id="db179-132">Data type</span></span> | <span data-ttu-id="db179-133">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="db179-133">Data context</span></span> | <span data-ttu-id="db179-134">Описание</span><span class="sxs-lookup"><span data-stu-id="db179-134">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="db179-135">`events`: список объектов Event</span><span class="sxs-lookup"><span data-stu-id="db179-135">`events`: list of event objects</span></span> | <span data-ttu-id="db179-136">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="db179-136">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="db179-137">`event`: объект Event</span><span class="sxs-lookup"><span data-stu-id="db179-137">`event`: event object</span></span> | <span data-ttu-id="db179-138">Шаблон, используемый для отображения каждого события.</span><span class="sxs-lookup"><span data-stu-id="db179-138">The template used to render each event.</span></span> |
| `header` | <span data-ttu-id="db179-139">`header`: строка</span><span class="sxs-lookup"><span data-stu-id="db179-139">`header`: string</span></span> | <span data-ttu-id="db179-140">Шаблон, используемый для отображения заголовка ежедневно.</span><span class="sxs-lookup"><span data-stu-id="db179-140">The template used to render the header for each day.</span></span> |
| `other` | <span data-ttu-id="db179-141">`event`: объект Event</span><span class="sxs-lookup"><span data-stu-id="db179-141">`event`: event object</span></span> | <span data-ttu-id="db179-142">Шаблон, используемый для отображения дополнительного содержимого для каждого события.</span><span class="sxs-lookup"><span data-stu-id="db179-142">The template used to render additional content for each event.</span></span> |
| `no-data` | <span data-ttu-id="db179-143">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="db179-143">No data context is passed</span></span> | <span data-ttu-id="db179-144">Шаблон, используемый при отсутствии доступных событий.</span><span class="sxs-lookup"><span data-stu-id="db179-144">The template used when no events are available.</span></span> |
| `loading` | <span data-ttu-id="db179-145">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="db179-145">No data context is passed</span></span> | <span data-ttu-id="db179-146">Шаблон, используемый при загрузке данных.</span><span class="sxs-lookup"><span data-stu-id="db179-146">The template used when data is loading.</span></span> |

<span data-ttu-id="db179-147">В следующих примерах показано, как использовать `event` шаблон:</span><span class="sxs-lookup"><span data-stu-id="db179-147">The following examples illustrates how to use the `event` template:</span></span>

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          show-name
          show-email>
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

<span data-ttu-id="db179-148">Чтобы узнать больше, ознакомьтесь со статьей [шаблоны](../templates.md).</span><span class="sxs-lookup"><span data-stu-id="db179-148">To learn more, see [templates](../templates.md).</span></span>

## <a name="graph-scopes"></a><span data-ttu-id="db179-149">Области диаграммы</span><span class="sxs-lookup"><span data-stu-id="db179-149">Graph scopes</span></span>

<span data-ttu-id="db179-150">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="db179-150">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="db179-151">resource</span><span class="sxs-lookup"><span data-stu-id="db179-151">resource</span></span> | <span data-ttu-id="db179-152">разрешение или область</span><span class="sxs-lookup"><span data-stu-id="db179-152">permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="db179-153">/ме/календарвиев</span><span class="sxs-lookup"><span data-stu-id="db179-153">/me/calendarview</span></span>](https://docs.microsoft.com/en-us/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

<span data-ttu-id="db179-154">Компонент позволяет указать другой запрос Microsoft Graph для вызова (например, `/groups/{id}/calendar/calendarView`).</span><span class="sxs-lookup"><span data-stu-id="db179-154">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="db179-155">В этом случае добавьте область в конец строки, отделенной`|`</span><span class="sxs-lookup"><span data-stu-id="db179-155">In this case, append the scope at the end of the string, delimited by `|`</span></span>

## <a name="authentication"></a><span data-ttu-id="db179-156">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="db179-156">Authentication</span></span>

<span data-ttu-id="db179-157">Элемент управления входом использует глобальную службу проверки подлинности, описанную в [документации по проверке](./../providers.md)подлинности.</span><span class="sxs-lookup"><span data-stu-id="db179-157">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

