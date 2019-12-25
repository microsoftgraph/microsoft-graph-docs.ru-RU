---
title: Компонент повестки в наборе инструментов Microsoft Graph
description: Веб-компонент "центр центровой связи" используется для представления событий в календаре пользователя или группы.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 0676c7ab66e899aa4af3dea0f623f301ce9b9f4e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866891"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="02cd5-103">Компонент повестки в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="02cd5-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="02cd5-104">`mgt-agenda` Веб-компонент представляет события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="02cd5-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="02cd5-105">По умолчанию в календаре отображаются текущие события пользователя, вошедшего в текущий день.</span><span class="sxs-lookup"><span data-stu-id="02cd5-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="02cd5-106">Компонент также может использовать любую конечную точку, возвращающую события из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="02cd5-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="02cd5-107">Пример</span><span class="sxs-lookup"><span data-stu-id="02cd5-107">Example</span></span>

[<span data-ttu-id="02cd5-108">Пример жсфиддле</span><span class="sxs-lookup"><span data-stu-id="02cd5-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![центр, повестка](./images/mgt-agenda.png)

## <a name="properties"></a><span data-ttu-id="02cd5-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="02cd5-110">Properties</span></span>

<span data-ttu-id="02cd5-111">По умолчанию `mgt-agenda` компонент получает события от `/me/calendarview` конечной точки и отображает события за текущий день.</span><span class="sxs-lookup"><span data-stu-id="02cd5-111">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="02cd5-112">Существует несколько свойств, которые можно использовать для изменения этого поведения.</span><span class="sxs-lookup"><span data-stu-id="02cd5-112">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="02cd5-113">Атрибут</span><span class="sxs-lookup"><span data-stu-id="02cd5-113">Attribute</span></span> | <span data-ttu-id="02cd5-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="02cd5-114">Property</span></span> | <span data-ttu-id="02cd5-115">Описание</span><span class="sxs-lookup"><span data-stu-id="02cd5-115">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="02cd5-116">дата</span><span class="sxs-lookup"><span data-stu-id="02cd5-116">date</span></span> | <span data-ttu-id="02cd5-117">date</span><span class="sxs-lookup"><span data-stu-id="02cd5-117">date</span></span> | <span data-ttu-id="02cd5-118">Строка, представляющая дату начала событий, которые необходимо получить из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="02cd5-118">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="02cd5-119">Значение должно быть в формате, который может быть проанализирован с помощью [конструктора Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -value, если `event-query` задан атрибут.</span><span class="sxs-lookup"><span data-stu-id="02cd5-119">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="02cd5-120">срок</span><span class="sxs-lookup"><span data-stu-id="02cd5-120">days</span></span> | <span data-ttu-id="02cd5-121">срок</span><span class="sxs-lookup"><span data-stu-id="02cd5-121">days</span></span> | <span data-ttu-id="02cd5-122">Число дней для выборки из Microsoft Graph — значение по умолчанию не оказывает никакого действия, если `event-query` задан атрибут.</span><span class="sxs-lookup"><span data-stu-id="02cd5-122">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="02cd5-123">Show — Max</span><span class="sxs-lookup"><span data-stu-id="02cd5-123">show-max</span></span> | <span data-ttu-id="02cd5-124">шовмакс</span><span class="sxs-lookup"><span data-stu-id="02cd5-124">showMax</span></span> | <span data-ttu-id="02cd5-125">Число, определяющее максимальное число отображаемых событий.</span><span class="sxs-lookup"><span data-stu-id="02cd5-125">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="02cd5-126">Значение по умолчанию не задано (максимальное значение не задано).</span><span class="sxs-lookup"><span data-stu-id="02cd5-126">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="02cd5-127">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="02cd5-127">group-id</span></span> | <span data-ttu-id="02cd5-128">groupId</span><span class="sxs-lookup"><span data-stu-id="02cd5-128">groupId</span></span> | <span data-ttu-id="02cd5-129">Идентификатор строки для календаря группы, который будет использоваться вместо текущего календаря пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="02cd5-129">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="02cd5-130">событие — запрос</span><span class="sxs-lookup"><span data-stu-id="02cd5-130">event-query</span></span> | <span data-ttu-id="02cd5-131">евенткуери</span><span class="sxs-lookup"><span data-stu-id="02cd5-131">eventQuery</span></span> | <span data-ttu-id="02cd5-132">Строка, представляющая альтернативный запрос, который будет использоваться при получении событий из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="02cd5-132">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="02cd5-133">При необходимости добавьте делегированную область в конец строки, чтобы она была ограничена `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span><span class="sxs-lookup"><span data-stu-id="02cd5-133">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="02cd5-134">Мероприятия</span><span class="sxs-lookup"><span data-stu-id="02cd5-134">events</span></span> | <span data-ttu-id="02cd5-135">Мероприятия</span><span class="sxs-lookup"><span data-stu-id="02cd5-135">events</span></span> | <span data-ttu-id="02cd5-136">Массив событий, чтобы получить или задать список событий, отображаемых компонентом, с помощью этого свойства можно получить доступ к событиям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="02cd5-136">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="02cd5-137">Присвойте этому значению значение загрузка собственных событий, если значение задано разработчиком, `date`атрибуты `days`, или `event-query` , атрибуты, не действуют.</span><span class="sxs-lookup"><span data-stu-id="02cd5-137">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="02cd5-138">Группировка по дням</span><span class="sxs-lookup"><span data-stu-id="02cd5-138">group-by-day</span></span> | <span data-ttu-id="02cd5-139">граупбидай</span><span class="sxs-lookup"><span data-stu-id="02cd5-139">groupByDay</span></span> | <span data-ttu-id="02cd5-140">Логическое значение для группировки событий по дням события по умолчанию не группируются.</span><span class="sxs-lookup"><span data-stu-id="02cd5-140">A Boolean value to group events by day - by default events are not grouped.</span></span> |

<span data-ttu-id="02cd5-141">В следующем примере показано, как изменить поведение компонента для извлечения данных за определенную дату и до трех дней.</span><span class="sxs-lookup"><span data-stu-id="02cd5-141">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="02cd5-142">В следующем примере показано изменение поведения компонента для извлечения данных из определенного запроса.</span><span class="sxs-lookup"><span data-stu-id="02cd5-142">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="02cd5-143">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="02cd5-143">CSS custom properties</span></span>

<span data-ttu-id="02cd5-144">`mgt-agenda` Компонент определяет следующие НАСТРАИВАЕМЫЕ свойства CSS</span><span class="sxs-lookup"><span data-stu-id="02cd5-144">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="02cd5-145">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="02cd5-145">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="02cd5-146">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="02cd5-146">Templates</span></span>

<span data-ttu-id="02cd5-147">`mgt-agenda` Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="02cd5-147">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="02cd5-148">Чтобы указать шаблон, включите `<template>` элемент в компонент и задайте для него `data-type` одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="02cd5-148">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="02cd5-149">Тип данных</span><span class="sxs-lookup"><span data-stu-id="02cd5-149">Data type</span></span> | <span data-ttu-id="02cd5-150">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="02cd5-150">Data context</span></span> | <span data-ttu-id="02cd5-151">Описание</span><span class="sxs-lookup"><span data-stu-id="02cd5-151">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="02cd5-152">`events`: список объектов Event</span><span class="sxs-lookup"><span data-stu-id="02cd5-152">`events`: list of event objects</span></span> | <span data-ttu-id="02cd5-153">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="02cd5-153">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="02cd5-154">`event`: объект Event</span><span class="sxs-lookup"><span data-stu-id="02cd5-154">`event`: event object</span></span> | <span data-ttu-id="02cd5-155">Шаблон, используемый для отображения каждого события.</span><span class="sxs-lookup"><span data-stu-id="02cd5-155">The template used to render each event.</span></span> |
| `header` | <span data-ttu-id="02cd5-156">`header`: строка</span><span class="sxs-lookup"><span data-stu-id="02cd5-156">`header`: string</span></span> | <span data-ttu-id="02cd5-157">Шаблон, используемый для отображения заголовка ежедневно.</span><span class="sxs-lookup"><span data-stu-id="02cd5-157">The template used to render the header for each day.</span></span> |
| `other` | <span data-ttu-id="02cd5-158">`event`: объект Event</span><span class="sxs-lookup"><span data-stu-id="02cd5-158">`event`: event object</span></span> | <span data-ttu-id="02cd5-159">Шаблон, используемый для отображения дополнительного содержимого для каждого события.</span><span class="sxs-lookup"><span data-stu-id="02cd5-159">The template used to render additional content for each event.</span></span> |
| `no-data` | <span data-ttu-id="02cd5-160">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="02cd5-160">No data context is passed</span></span> | <span data-ttu-id="02cd5-161">Шаблон, используемый при отсутствии доступных событий.</span><span class="sxs-lookup"><span data-stu-id="02cd5-161">The template used when no events are available.</span></span> |
| `loading` | <span data-ttu-id="02cd5-162">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="02cd5-162">No data context is passed</span></span> | <span data-ttu-id="02cd5-163">Шаблон, используемый при загрузке данных.</span><span class="sxs-lookup"><span data-stu-id="02cd5-163">The template used when data is loading.</span></span> |

<span data-ttu-id="02cd5-164">В следующих примерах показано, как использовать `event` шаблон:</span><span class="sxs-lookup"><span data-stu-id="02cd5-164">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="02cd5-165">Чтобы узнать больше, ознакомьтесь со статьей [шаблоны](../templates.md).</span><span class="sxs-lookup"><span data-stu-id="02cd5-165">To learn more, see [templates](../templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="02cd5-166">События</span><span class="sxs-lookup"><span data-stu-id="02cd5-166">Events</span></span>

<span data-ttu-id="02cd5-167">Из элемента управления запускаются следующие события.</span><span class="sxs-lookup"><span data-stu-id="02cd5-167">The following events are fired from the control.</span></span>

| <span data-ttu-id="02cd5-168">Событие</span><span class="sxs-lookup"><span data-stu-id="02cd5-168">Event</span></span> | <span data-ttu-id="02cd5-169">Описание</span><span class="sxs-lookup"><span data-stu-id="02cd5-169">Description</span></span> |
| --- | --- |
| <span data-ttu-id="02cd5-170">евенткликк</span><span class="sxs-lookup"><span data-stu-id="02cd5-170">eventClick</span></span> | <span data-ttu-id="02cd5-171">Пользователь щелкает или нажимает событие.</span><span class="sxs-lookup"><span data-stu-id="02cd5-171">The user clicks or taps on an event.</span></span>|


## <a name="graph-scopes"></a><span data-ttu-id="02cd5-172">Области диаграммы</span><span class="sxs-lookup"><span data-stu-id="02cd5-172">Graph scopes</span></span>

<span data-ttu-id="02cd5-173">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="02cd5-173">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="02cd5-174">resource</span><span class="sxs-lookup"><span data-stu-id="02cd5-174">resource</span></span> | <span data-ttu-id="02cd5-175">разрешение или область</span><span class="sxs-lookup"><span data-stu-id="02cd5-175">permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="02cd5-176">/ме/календарвиев</span><span class="sxs-lookup"><span data-stu-id="02cd5-176">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

<span data-ttu-id="02cd5-177">Компонент позволяет указать другой запрос Microsoft Graph для вызова (например, `/groups/{id}/calendar/calendarView`).</span><span class="sxs-lookup"><span data-stu-id="02cd5-177">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="02cd5-178">В этом случае добавьте область в конец строки, отделенной`|`</span><span class="sxs-lookup"><span data-stu-id="02cd5-178">In this case, append the scope at the end of the string, delimited by `|`</span></span>

## <a name="authentication"></a><span data-ttu-id="02cd5-179">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="02cd5-179">Authentication</span></span>

<span data-ttu-id="02cd5-180">Элемент управления входом использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="02cd5-180">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

