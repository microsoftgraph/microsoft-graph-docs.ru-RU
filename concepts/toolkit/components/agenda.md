---
title: Компонент "Повестка дня" в Microsoft Graph Toolkit
description: Веб-компонент mgt-agenda используется для представления событий в календаре пользователя или группы.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 394f5dee6c8bf6f81b68d3b0b8c8cb1d73ef06ef
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082337"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1b3d8-103">Компонент "Повестка дня" в Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="1b3d8-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1b3d8-104">Веб-компонент `mgt-agenda` отображает события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="1b3d8-105">По умолчанию в календаре отображаются текущие события вошедшего пользователя, запланированные на текущий день.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="1b3d8-106">Компонент также может использовать любую конечную точку, возвращающую события из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="1b3d8-107">Пример</span><span class="sxs-lookup"><span data-stu-id="1b3d8-107">Example</span></span>

<span data-ttu-id="1b3d8-108">В следующем примере показаны события календаря вошедшего пользователя, отображаемые с помощью компонента `mgt-agenda`.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="1b3d8-109">Вы можете использовать редактор кода, чтобы узнать, как [свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="1b3d8-110">Открыть этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="1b3d8-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="1b3d8-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b3d8-111">Properties</span></span>

<span data-ttu-id="1b3d8-112">По умолчанию компонент `mgt-agenda` извлекает события из конечной точки `/me/calendarview` и отображает события, запланированные на текущий день.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="1b3d8-113">Это поведение можно изменить с помощью нескольких свойств.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="1b3d8-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="1b3d8-114">Attribute</span></span> | <span data-ttu-id="1b3d8-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b3d8-115">Property</span></span> | <span data-ttu-id="1b3d8-116">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3d8-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1b3d8-117">дата</span><span class="sxs-lookup"><span data-stu-id="1b3d8-117">date</span></span> | <span data-ttu-id="1b3d8-118">date</span><span class="sxs-lookup"><span data-stu-id="1b3d8-118">date</span></span> | <span data-ttu-id="1b3d8-119">Строка, представляющая дату начала событий, извлекаемых из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="1b3d8-120">Значение должно быть в формате, который может быть проанализирован [конструктором дат](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date). Значение не оказывает влияния, если установлен атрибут `event-query`.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="1b3d8-121">days</span><span class="sxs-lookup"><span data-stu-id="1b3d8-121">days</span></span> | <span data-ttu-id="1b3d8-122">days</span><span class="sxs-lookup"><span data-stu-id="1b3d8-122">days</span></span> | <span data-ttu-id="1b3d8-123">Количество дней, извлекаемых из Microsoft Graph (по умолчанию — 3 дня). Значение не оказывает влияния, если установлен атрибут `event-query`.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="1b3d8-124">show-max</span><span class="sxs-lookup"><span data-stu-id="1b3d8-124">show-max</span></span> | <span data-ttu-id="1b3d8-125">showMax</span><span class="sxs-lookup"><span data-stu-id="1b3d8-125">showMax</span></span> | <span data-ttu-id="1b3d8-126">Число, указывающее максимальное количество отображаемых событий.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="1b3d8-127">Значение по умолчанию не установлено (не ограничено).</span><span class="sxs-lookup"><span data-stu-id="1b3d8-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="1b3d8-128">group-id</span><span class="sxs-lookup"><span data-stu-id="1b3d8-128">group-id</span></span> | <span data-ttu-id="1b3d8-129">groupId</span><span class="sxs-lookup"><span data-stu-id="1b3d8-129">groupId</span></span> | <span data-ttu-id="1b3d8-130">Идентификатор строки для группового календаря, используемого вместо текущего календаря вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="1b3d8-131">event-query</span><span class="sxs-lookup"><span data-stu-id="1b3d8-131">event-query</span></span> | <span data-ttu-id="1b3d8-132">eventQuery</span><span class="sxs-lookup"><span data-stu-id="1b3d8-132">eventQuery</span></span> | <span data-ttu-id="1b3d8-133">Строка, представляющая альтернативный запрос, используемый при извлечении событий из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="1b3d8-134">При необходимости добавьте делегированную область в конец строки, разделив ее с помощью символа `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span><span class="sxs-lookup"><span data-stu-id="1b3d8-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="1b3d8-135">events</span><span class="sxs-lookup"><span data-stu-id="1b3d8-135">events</span></span> | <span data-ttu-id="1b3d8-136">events</span><span class="sxs-lookup"><span data-stu-id="1b3d8-136">events</span></span> | <span data-ttu-id="1b3d8-137">Массив событий для получения или установки списка событий, отображаемых компонентом. Используйте это свойство для доступа к событиям, загружаемым компонентом.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="1b3d8-138">Установите это значение, чтобы загрузить свои собственные события. Если значение установлено разработчиком, атрибуты `date`, `days` и `event-query` не оказывают влияния.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="1b3d8-139">group-by-day</span><span class="sxs-lookup"><span data-stu-id="1b3d8-139">group-by-day</span></span> | <span data-ttu-id="1b3d8-140">groupByDay</span><span class="sxs-lookup"><span data-stu-id="1b3d8-140">groupByDay</span></span> | <span data-ttu-id="1b3d8-141">Логическое значение для группировки событий по дням (по умолчанию события не группируются).</span><span class="sxs-lookup"><span data-stu-id="1b3d8-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| <span data-ttu-id="1b3d8-142">preferred-timezone</span><span class="sxs-lookup"><span data-stu-id="1b3d8-142">preferred-timezone</span></span> | <span data-ttu-id="1b3d8-143">preferredTimezone</span><span class="sxs-lookup"><span data-stu-id="1b3d8-143">preferredTimezone</span></span> | <span data-ttu-id="1b3d8-144">Имя предпочтительного часового пояса, используемого при извлечении событий из Microsoft Graph. Например, `Pacific Standard Time`.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-144">Name of the preferred time zone to use when retrieving events from Microsoft Graph; for example, `Pacific Standard Time`.</span></span> <span data-ttu-id="1b3d8-145">По умолчанию этот атрибут использует время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-145">By default, this attribute uses the UTC time zone.</span></span> <span data-ttu-id="1b3d8-146">Предпочтительный часовой пояс для текущего пользователя можно получить, вызвав конечную точку `me/mailboxSettings` и прочитав значение свойства **timeZone**.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-146">The preferred time zone for the current user can be retrieved by calling the `me/mailboxSettings` endpoint and reading the value of the **timeZone** property.</span></span> |

<span data-ttu-id="1b3d8-147">Следующий пример демонстрирует изменение поведения компонента для извлечения данных за определенную дату и до трех дней.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-147">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="1b3d8-148">Следующий пример демонстрирует изменение поведения компонента для извлечения данных из определенного запроса.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-148">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="methods"></a><span data-ttu-id="1b3d8-149">Методы</span><span class="sxs-lookup"><span data-stu-id="1b3d8-149">Methods</span></span>
| <span data-ttu-id="1b3d8-150">Метод</span><span class="sxs-lookup"><span data-stu-id="1b3d8-150">Method</span></span> | <span data-ttu-id="1b3d8-151">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3d8-151">Description</span></span> |
| --- | --- |
| <span data-ttu-id="1b3d8-152">reload()</span><span class="sxs-lookup"><span data-stu-id="1b3d8-152">reload()</span></span> | <span data-ttu-id="1b3d8-153">Вызывает метод для перезагрузки компонента с потенциальными новыми данными на основе его свойств.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-153">Call the method to reload the component with potential new data based on its properties.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="1b3d8-154">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="1b3d8-154">CSS custom properties</span></span>

<span data-ttu-id="1b3d8-155">Компонент `mgt-agenda` определяет следующие настраиваемые свойства CSS.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-155">The `mgt-agenda` component defines these CSS custom properties</span></span>

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background-color: #ffffff;
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

<span data-ttu-id="1b3d8-156">Дополнительные сведения см. в статье [Компоненты стиля](../customize-components/style.md).</span><span class="sxs-lookup"><span data-stu-id="1b3d8-156">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="1b3d8-157">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="1b3d8-157">Templates</span></span>

<span data-ttu-id="1b3d8-158">Компонент `mgt-agenda` поддерживает несколько [шаблонов](../customize-components/templates.md), позволяющих заменить его определенные части.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-158">The `mgt-agenda` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="1b3d8-159">Чтобы указать шаблон, добавьте элемент `<template>` в компонент и присвойте параметру `data-type` одно из следующих значений.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-159">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="1b3d8-160">Тип данных</span><span class="sxs-lookup"><span data-stu-id="1b3d8-160">Data type</span></span> | <span data-ttu-id="1b3d8-161">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="1b3d8-161">Data context</span></span> | <span data-ttu-id="1b3d8-162">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3d8-162">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="1b3d8-163">`events`: список объектов события</span><span class="sxs-lookup"><span data-stu-id="1b3d8-163">`events`: list of event objects</span></span> | <span data-ttu-id="1b3d8-164">Шаблон по умолчанию заменяет весь компонент вашим собственным компонентом.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-164">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="1b3d8-165">`event`: объект события</span><span class="sxs-lookup"><span data-stu-id="1b3d8-165">`event`: event object</span></span> | <span data-ttu-id="1b3d8-166">Шаблон, используемый для отображения каждого события.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-166">The template used to render each event.</span></span> |
| `event-other` | <span data-ttu-id="1b3d8-167">`event`: объект события</span><span class="sxs-lookup"><span data-stu-id="1b3d8-167">`event`: event object</span></span> | <span data-ttu-id="1b3d8-168">Шаблон, используемый для отображения дополнительного содержимого для каждого события.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-168">The template used to render additional content for each event.</span></span> |
| `header` | <span data-ttu-id="1b3d8-169">`header`: строка</span><span class="sxs-lookup"><span data-stu-id="1b3d8-169">`header`: string</span></span> | <span data-ttu-id="1b3d8-170">Шаблон, используемый для отображения заголовка для каждого дня.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-170">The template used to render the header for each day.</span></span> |
| `loading` | <span data-ttu-id="1b3d8-171">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="1b3d8-171">No data context is passed</span></span> | <span data-ttu-id="1b3d8-172">Шаблон, используемый при загрузке данных.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-172">The template used when data is loading.</span></span> |
| `no-data` | <span data-ttu-id="1b3d8-173">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="1b3d8-173">No data context is passed</span></span> | <span data-ttu-id="1b3d8-174">Шаблон, используемый при отсутствии событий.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-174">The template used when no events are available.</span></span> |

<span data-ttu-id="1b3d8-175">В следующих примерах показано, как использовать шаблон `event`.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-175">The following examples illustrates how to use the `event` template:</span></span>

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          view="twolines">
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

<span data-ttu-id="1b3d8-176">Дополнительные сведения см. в статье [Шаблоны](../customize-components/templates.md).</span><span class="sxs-lookup"><span data-stu-id="1b3d8-176">To learn more, see [templates](../customize-components/templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="1b3d8-177">События</span><span class="sxs-lookup"><span data-stu-id="1b3d8-177">Events</span></span>

<span data-ttu-id="1b3d8-178">Из элемента управления инициируются следующие события.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-178">The following events are fired from the control.</span></span>

| <span data-ttu-id="1b3d8-179">Событие</span><span class="sxs-lookup"><span data-stu-id="1b3d8-179">Event</span></span> | <span data-ttu-id="1b3d8-180">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3d8-180">Description</span></span> |
| --- | --- |
| `eventClick` | <span data-ttu-id="1b3d8-181">Пользователь щелкает или нажимает событие.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-181">The user clicks or taps an event.</span></span>|

<span data-ttu-id="1b3d8-182">Дополнительные сведения об обработке событий см. в [этой работе.](../customize-components/events.md)</span><span class="sxs-lookup"><span data-stu-id="1b3d8-182">For more information about handling events, see [events](../customize-components/events.md).</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="1b3d8-183">Разрешения Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1b3d8-183">Microsoft Graph permissions</span></span>

<span data-ttu-id="1b3d8-184">Этот компонент использует следующие API и разрешения Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-184">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="1b3d8-185">Настройка</span><span class="sxs-lookup"><span data-stu-id="1b3d8-185">Configuration</span></span> | <span data-ttu-id="1b3d8-186">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1b3d8-186">Permission</span></span> | <span data-ttu-id="1b3d8-187">API</span><span class="sxs-lookup"><span data-stu-id="1b3d8-187">API</span></span>
| - | - | - |
| <span data-ttu-id="1b3d8-188">default</span><span class="sxs-lookup"><span data-stu-id="1b3d8-188">default</span></span> | <span data-ttu-id="1b3d8-189">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1b3d8-189">Calendars.Read</span></span> | [<span data-ttu-id="1b3d8-190">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="1b3d8-190">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview) |

<span data-ttu-id="1b3d8-191">Компонент позволяет указать другой запрос Microsoft Graph для вызова (например, `/groups/{id}/calendar/calendarView`).</span><span class="sxs-lookup"><span data-stu-id="1b3d8-191">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="1b3d8-192">В этом случае добавьте разрешение в конец строки, разделенной символом `|`.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-192">In this case, append the permission to the end of the string, delimited by `|`.</span></span>

<span data-ttu-id="1b3d8-193">При использовании шаблона по умолчанию и шаблона по умолчанию `renderAttendees`, требуются дополнительные API и разрешения.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-193">When using the default template and default `renderAttendees` template, additional APIs and permissions are required.</span></span> <span data-ttu-id="1b3d8-194">Шаблон по умолчанию для этого компонента использует компонент [mgt-people](people.md) для событий, в которых есть участники, и наследует все разрешения.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-194">The default template for this component uses a [mgt-people](people.md) component for events that have attendees, and inherits all permissions.</span></span>

## <a name="authentication"></a><span data-ttu-id="1b3d8-195">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="1b3d8-195">Authentication</span></span>

<span data-ttu-id="1b3d8-196">В элементе управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности](../providers/providers.md).</span><span class="sxs-lookup"><span data-stu-id="1b3d8-196">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="cache"></a><span data-ttu-id="1b3d8-197">Кэш</span><span class="sxs-lookup"><span data-stu-id="1b3d8-197">Cache</span></span>

<span data-ttu-id="1b3d8-198">Компонент `mgt-agenda` не кэшет данных.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-198">The `mgt-agenda` component doesn't cache any data.</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="1b3d8-199">Расширение для дополнительного управления</span><span class="sxs-lookup"><span data-stu-id="1b3d8-199">Extend for more control</span></span>

<span data-ttu-id="1b3d8-200">В более сложных сценариях или настраиваемых пользовательских интерфейсах этот компонент предоставляет несколько методов `protected` render\* для переопределения в расширениях компонента.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-200">For more complex scenarios or a truly custom UX, this component exposes several `protected` render\* methods for override in component extensions.</span></span>

| <span data-ttu-id="1b3d8-201">Метод</span><span class="sxs-lookup"><span data-stu-id="1b3d8-201">Method</span></span> | <span data-ttu-id="1b3d8-202">Описание</span><span class="sxs-lookup"><span data-stu-id="1b3d8-202">Description</span></span> |
| - | - |
| <span data-ttu-id="1b3d8-203">renderLoading</span><span class="sxs-lookup"><span data-stu-id="1b3d8-203">renderLoading</span></span> | <span data-ttu-id="1b3d8-204">Отображает состояние загрузки во время загрузки компонента.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-204">Renders a loading state while the component loads.</span></span> |
| <span data-ttu-id="1b3d8-205">renderNoData</span><span class="sxs-lookup"><span data-stu-id="1b3d8-205">renderNoData</span></span> | <span data-ttu-id="1b3d8-206">Отображает пустое состояние данных.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-206">Renders an empty data state.</span></span> |
| <span data-ttu-id="1b3d8-207">renderGroups</span><span class="sxs-lookup"><span data-stu-id="1b3d8-207">renderGroups</span></span> | <span data-ttu-id="1b3d8-208">Сортирует данные событий по группам и отображает их с заголовками групп.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-208">Sorts event data into groups and renders them with group headers.</span></span> |
| <span data-ttu-id="1b3d8-209">renderHeader</span><span class="sxs-lookup"><span data-stu-id="1b3d8-209">renderHeader</span></span> | <span data-ttu-id="1b3d8-210">Отображает заголовок группы.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-210">Renders a group header.</span></span> |
| <span data-ttu-id="1b3d8-211">renderEvents</span><span class="sxs-lookup"><span data-stu-id="1b3d8-211">renderEvents</span></span> | <span data-ttu-id="1b3d8-212">Отображает список объектов события.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-212">Renders a list of event objects.</span></span> |
| <span data-ttu-id="1b3d8-213">renderEvent</span><span class="sxs-lookup"><span data-stu-id="1b3d8-213">renderEvent</span></span> | <span data-ttu-id="1b3d8-214">Отображает одно событие и все его части.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-214">Renders a singular event and all of its parts.</span></span>
| <span data-ttu-id="1b3d8-215">renderTitle</span><span class="sxs-lookup"><span data-stu-id="1b3d8-215">renderTitle</span></span> | <span data-ttu-id="1b3d8-216">Отображает название события.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-216">Renders the event title part.</span></span> |
| <span data-ttu-id="1b3d8-217">renderLocation</span><span class="sxs-lookup"><span data-stu-id="1b3d8-217">renderLocation</span></span> | <span data-ttu-id="1b3d8-218">Отображает расположение события.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-218">Renders the event location part.</span></span> |
| <span data-ttu-id="1b3d8-219">renderAttendees</span><span class="sxs-lookup"><span data-stu-id="1b3d8-219">renderAttendees</span></span> | <span data-ttu-id="1b3d8-220">Отображает участников события.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-220">Renders the event attendees part.</span></span> |
| <span data-ttu-id="1b3d8-221">renderOther</span><span class="sxs-lookup"><span data-stu-id="1b3d8-221">renderOther</span></span> | <span data-ttu-id="1b3d8-222">Отображает дополнительное содержимое события.</span><span class="sxs-lookup"><span data-stu-id="1b3d8-222">Renders additional event content.</span></span> |
