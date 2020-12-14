---
title: Компонент "Повестка дня" в microsoft Graph набор средств
description: Веб-компонент mgt-agenda используется для представления событий в календаре пользователя или группы.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: e66ffed1f10de5c4c9b9b322d9070074ec707000
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659550"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="1b6d4-103">Компонент "Повестка дня" в microsoft Graph набор средств</span><span class="sxs-lookup"><span data-stu-id="1b6d4-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="1b6d4-104">`mgt-agenda`Веб-компонент представляет события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="1b6d4-105">По умолчанию в календаре отображаются текущие события, в которые были вписались пользователи за текущий день.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="1b6d4-106">Компонент также может использовать любую конечную точку, которая возвращает события из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="1b6d4-107">Пример</span><span class="sxs-lookup"><span data-stu-id="1b6d4-107">Example</span></span>

<span data-ttu-id="1b6d4-108">В следующем примере показаны события календаря пользователя, выписав его с помощью `mgt-agenda` компонента.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="1b6d4-109">С помощью редактора кода можно [увидеть,](#properties) как свойства изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="1b6d4-110">Откройте этот пример в mgt.dev</span><span class="sxs-lookup"><span data-stu-id="1b6d4-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="1b6d4-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b6d4-111">Properties</span></span>

<span data-ttu-id="1b6d4-112">По умолчанию компонент получает события из конечной точки и отображает события `mgt-agenda` `/me/calendarview` за текущий день.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="1b6d4-113">Существует несколько свойств, которые можно использовать для изменения этого поведения.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="1b6d4-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="1b6d4-114">Attribute</span></span> | <span data-ttu-id="1b6d4-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b6d4-115">Property</span></span> | <span data-ttu-id="1b6d4-116">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6d4-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="1b6d4-117">дата</span><span class="sxs-lookup"><span data-stu-id="1b6d4-117">date</span></span> | <span data-ttu-id="1b6d4-118">date</span><span class="sxs-lookup"><span data-stu-id="1b6d4-118">date</span></span> | <span data-ttu-id="1b6d4-119">Строка, представляючная дату начала событий, извлекаемой из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="1b6d4-120">Значение должно быть в формате, который может быть разбор с помощью конструктора [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) — значение не имеет эффекта, если `event-query` атрибут установлен.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="1b6d4-121">days</span><span class="sxs-lookup"><span data-stu-id="1b6d4-121">days</span></span> | <span data-ttu-id="1b6d4-122">days</span><span class="sxs-lookup"><span data-stu-id="1b6d4-122">days</span></span> | <span data-ttu-id="1b6d4-123">Количество дней, за которые необходимо получить данные из Microsoft Graph (значение по умолчанию — 3), не влияет на значение, если `event-query` за установлен атрибут.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="1b6d4-124">show-max</span><span class="sxs-lookup"><span data-stu-id="1b6d4-124">show-max</span></span> | <span data-ttu-id="1b6d4-125">showMax</span><span class="sxs-lookup"><span data-stu-id="1b6d4-125">showMax</span></span> | <span data-ttu-id="1b6d4-126">Число, чтобы указать максимальное число событий для показа.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="1b6d4-127">Значение по умолчанию не за установлено (не максимальное значение).</span><span class="sxs-lookup"><span data-stu-id="1b6d4-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="1b6d4-128">group-id</span><span class="sxs-lookup"><span data-stu-id="1b6d4-128">group-id</span></span> | <span data-ttu-id="1b6d4-129">groupId</span><span class="sxs-lookup"><span data-stu-id="1b6d4-129">groupId</span></span> | <span data-ttu-id="1b6d4-130">ИД строки для календаря группы вместо текущего календаря пользователя, выписав его.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="1b6d4-131">event-query</span><span class="sxs-lookup"><span data-stu-id="1b6d4-131">event-query</span></span> | <span data-ttu-id="1b6d4-132">eventQuery</span><span class="sxs-lookup"><span data-stu-id="1b6d4-132">eventQuery</span></span> | <span data-ttu-id="1b6d4-133">Строка, представляютив альтернативный запрос, используемый при извлечении событий из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="1b6d4-134">При желании добавьте делегированную область в конце строки, делегированием ее с `|` помощью ( `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` ).</span><span class="sxs-lookup"><span data-stu-id="1b6d4-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="1b6d4-135">events</span><span class="sxs-lookup"><span data-stu-id="1b6d4-135">events</span></span> | <span data-ttu-id="1b6d4-136">events</span><span class="sxs-lookup"><span data-stu-id="1b6d4-136">events</span></span> | <span data-ttu-id="1b6d4-137">Массив событий, чтобы получить или установить список событий, отрисовки компонента . Используйте это свойство для доступа к событиям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="1b6d4-138">Установите это значение для загрузки собственных событий — если значение за установлено разработчиком, атрибуты `date` , или не имеют `days` `event-query` эффекта.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="1b6d4-139">группировка по дням</span><span class="sxs-lookup"><span data-stu-id="1b6d4-139">group-by-day</span></span> | <span data-ttu-id="1b6d4-140">groupByDay</span><span class="sxs-lookup"><span data-stu-id="1b6d4-140">groupByDay</span></span> | <span data-ttu-id="1b6d4-141">Boolean value to group events by day - by default events are not grouped.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| <span data-ttu-id="1b6d4-142">preferred-timezone</span><span class="sxs-lookup"><span data-stu-id="1b6d4-142">preferred-timezone</span></span> | <span data-ttu-id="1b6d4-143">preferredTimezone</span><span class="sxs-lookup"><span data-stu-id="1b6d4-143">preferredTimezone</span></span> | <span data-ttu-id="1b6d4-144">Имя предпочтительного часового пояса, используемого при искомом событиях из Microsoft Graph; например, `Pacific Standard Time` .</span><span class="sxs-lookup"><span data-stu-id="1b6d4-144">Name of the preferred time zone to use when retrieving events from Microsoft Graph; for example, `Pacific Standard Time`.</span></span> <span data-ttu-id="1b6d4-145">По умолчанию этот атрибут использует часовой пояс UTC.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-145">By default, this attribute uses the UTC time zone.</span></span> <span data-ttu-id="1b6d4-146">Предпочтительный часовой пояс для текущего пользователя можно получить, вызывая конечную точку и считывая значение `me/mailboxSettings` **свойства timeZone.**</span><span class="sxs-lookup"><span data-stu-id="1b6d4-146">The preferred time zone for the current user can be retrieved by calling the `me/mailboxSettings` endpoint and reading the value of the **timeZone** property.</span></span> |

<span data-ttu-id="1b6d4-147">В следующем примере изменяется поведение компонента для получения данных за определенную дату и до трех дней.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-147">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="1b6d4-148">В следующем примере изменяется поведение компонента для получения данных из определенного запроса.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-148">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="methods"></a><span data-ttu-id="1b6d4-149">Методы</span><span class="sxs-lookup"><span data-stu-id="1b6d4-149">Methods</span></span>
| <span data-ttu-id="1b6d4-150">Метод</span><span class="sxs-lookup"><span data-stu-id="1b6d4-150">Method</span></span> | <span data-ttu-id="1b6d4-151">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6d4-151">Description</span></span> |
| --- | --- |
| <span data-ttu-id="1b6d4-152">reload()</span><span class="sxs-lookup"><span data-stu-id="1b6d4-152">reload()</span></span> | <span data-ttu-id="1b6d4-153">Вызовите метод, чтобы перезагрузить компонент с потенциальными новыми данными на основе его свойств.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-153">Call the method to reload the component with potential new data based on its properties.</span></span> |

## <a name="css-custom-properties"></a><span data-ttu-id="1b6d4-154">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="1b6d4-154">CSS custom properties</span></span>

<span data-ttu-id="1b6d4-155">Компонент `mgt-agenda` определяет эти настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="1b6d4-155">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="1b6d4-156">Дополнительные узнать см. [в компонентах стиля.](../customize-components/style.md)</span><span class="sxs-lookup"><span data-stu-id="1b6d4-156">To learn more, see [styling components](../customize-components/style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="1b6d4-157">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="1b6d4-157">Templates</span></span>

<span data-ttu-id="1b6d4-158">Компонент `mgt-agenda` поддерживает несколько [шаблонов,](../customize-components/templates.md) которые позволяют заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-158">The `mgt-agenda` component supports several [templates](../customize-components/templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="1b6d4-159">Чтобы указать шаблон, включив элемент в компонент и заключив в него одно `<template>` `data-type` из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="1b6d4-159">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="1b6d4-160">Тип данных</span><span class="sxs-lookup"><span data-stu-id="1b6d4-160">Data type</span></span> | <span data-ttu-id="1b6d4-161">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="1b6d4-161">Data context</span></span> | <span data-ttu-id="1b6d4-162">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6d4-162">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="1b6d4-163">`events`: список объектов событий</span><span class="sxs-lookup"><span data-stu-id="1b6d4-163">`events`: list of event objects</span></span> | <span data-ttu-id="1b6d4-164">Шаблон по умолчанию заменяет весь компонент на собственный.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-164">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="1b6d4-165">`event`: объект event</span><span class="sxs-lookup"><span data-stu-id="1b6d4-165">`event`: event object</span></span> | <span data-ttu-id="1b6d4-166">Шаблон, используемый для отображения каждого события.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-166">The template used to render each event.</span></span> |
| `event-other` | <span data-ttu-id="1b6d4-167">`event`: объект event</span><span class="sxs-lookup"><span data-stu-id="1b6d4-167">`event`: event object</span></span> | <span data-ttu-id="1b6d4-168">Шаблон, используемый для отображения дополнительного содержимого для каждого события.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-168">The template used to render additional content for each event.</span></span> |
| `header` | <span data-ttu-id="1b6d4-169">`header`: string</span><span class="sxs-lookup"><span data-stu-id="1b6d4-169">`header`: string</span></span> | <span data-ttu-id="1b6d4-170">Шаблон, используемый для отображения загона для каждого дня.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-170">The template used to render the header for each day.</span></span> |
| `loading` | <span data-ttu-id="1b6d4-171">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="1b6d4-171">No data context is passed</span></span> | <span data-ttu-id="1b6d4-172">Шаблон, используемый при загрузке данных.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-172">The template used when data is loading.</span></span> |
| `no-data` | <span data-ttu-id="1b6d4-173">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="1b6d4-173">No data context is passed</span></span> | <span data-ttu-id="1b6d4-174">Шаблон, используемый, когда события недоступны.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-174">The template used when no events are available.</span></span> |

<span data-ttu-id="1b6d4-175">В следующих примерах показано, как использовать `event` шаблон:</span><span class="sxs-lookup"><span data-stu-id="1b6d4-175">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="1b6d4-176">Дополнительные узнать см. [в шаблонах.](../customize-components/templates.md)</span><span class="sxs-lookup"><span data-stu-id="1b6d4-176">To learn more, see [templates](../customize-components/templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="1b6d4-177">События</span><span class="sxs-lookup"><span data-stu-id="1b6d4-177">Events</span></span>

<span data-ttu-id="1b6d4-178">Из этого управления и происходят следующие события.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-178">The following events are fired from the control.</span></span>

| <span data-ttu-id="1b6d4-179">Событие</span><span class="sxs-lookup"><span data-stu-id="1b6d4-179">Event</span></span> | <span data-ttu-id="1b6d4-180">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6d4-180">Description</span></span> |
| --- | --- |
| <span data-ttu-id="1b6d4-181">eventClick</span><span class="sxs-lookup"><span data-stu-id="1b6d4-181">eventClick</span></span> | <span data-ttu-id="1b6d4-182">Пользователь щелкает или кжимает событие.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-182">The user clicks or taps an event.</span></span>|

## <a name="permissions"></a><span data-ttu-id="1b6d4-183">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b6d4-183">Permissions</span></span>

<span data-ttu-id="1b6d4-184">Этот компонент использует следующие API Microsoft Graph и разрешения:</span><span class="sxs-lookup"><span data-stu-id="1b6d4-184">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="1b6d4-185">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1b6d4-185">Resource</span></span> | <span data-ttu-id="1b6d4-186">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1b6d4-186">Permission</span></span> |
| - | - |
| [<span data-ttu-id="1b6d4-187">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="1b6d4-187">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview) | <span data-ttu-id="1b6d4-188">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="1b6d4-188">Calendars.Read</span></span> |

<span data-ttu-id="1b6d4-189">Компонент позволяет указать другой запрос Microsoft Graph для вызова `/groups/{id}/calendar/calendarView` (например, ).</span><span class="sxs-lookup"><span data-stu-id="1b6d4-189">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="1b6d4-190">В этом случае примените разрешение в конец строки с делегированный по `|` .</span><span class="sxs-lookup"><span data-stu-id="1b6d4-190">In this case, append the permission to the end of the string, delimited by `|`.</span></span>

<span data-ttu-id="1b6d4-191">При использовании шаблона по умолчанию и шаблона по умолчанию требуются дополнительные API и `renderAttendees` разрешения.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-191">When using the default template and default `renderAttendees` template, additional APIs and permissions are required.</span></span> <span data-ttu-id="1b6d4-192">Шаблон по умолчанию для этого компонента использует компонент [mgt-people](people.md) для событий с участниками, для чего требуется следующее.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-192">The default template for this component uses a [mgt-people](people.md) component for events that have attendees, which requires the following.</span></span>

| <span data-ttu-id="1b6d4-193">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1b6d4-193">Resource</span></span> | <span data-ttu-id="1b6d4-194">Разрешение</span><span class="sxs-lookup"><span data-stu-id="1b6d4-194">Permission</span></span> |
| - | - |
| [<span data-ttu-id="1b6d4-195">/users</span><span class="sxs-lookup"><span data-stu-id="1b6d4-195">/users</span></span>](/graph/api/user-list) | <span data-ttu-id="1b6d4-196">Users.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1b6d4-196">Users.ReadBasic.All</span></span> |
| [<span data-ttu-id="1b6d4-197">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="1b6d4-197">/me/calendarview</span></span>](/graph/api/user-list-people) | <span data-ttu-id="1b6d4-198">People.Read</span><span class="sxs-lookup"><span data-stu-id="1b6d4-198">People.Read</span></span> |
| [<span data-ttu-id="1b6d4-199">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="1b6d4-199">/me/calendarview</span></span>](/graph/api/user-list-contacts) | <span data-ttu-id="1b6d4-200">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="1b6d4-200">Contacts.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="1b6d4-201">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="1b6d4-201">Authentication</span></span>

<span data-ttu-id="1b6d4-202">Для управления входом используется глобальный поставщик проверки подлинности, описанный в [документации по проверке подлинности.](../providers/providers.md)</span><span class="sxs-lookup"><span data-stu-id="1b6d4-202">The login control uses the global authentication provider described in the [authentication documentation](../providers/providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="1b6d4-203">Расширение для большего контроля</span><span class="sxs-lookup"><span data-stu-id="1b6d4-203">Extend for more control</span></span>

<span data-ttu-id="1b6d4-204">Для более сложных сценариев или по-настоящему настраиваемого пользовательского пользовательского управления этот компонент предоставляет несколько методов render\* для переопределения `protected` в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-204">For more complex scenarios or a truly custom UX, this component exposes several `protected` render\* methods for override in component extensions.</span></span>

| <span data-ttu-id="1b6d4-205">Метод</span><span class="sxs-lookup"><span data-stu-id="1b6d4-205">Method</span></span> | <span data-ttu-id="1b6d4-206">Описание</span><span class="sxs-lookup"><span data-stu-id="1b6d4-206">Description</span></span> |
| - | - |
| <span data-ttu-id="1b6d4-207">renderLoading</span><span class="sxs-lookup"><span data-stu-id="1b6d4-207">renderLoading</span></span> | <span data-ttu-id="1b6d4-208">Отрисовка состояния загрузки во время загрузки компонента.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-208">Renders a loading state while the component loads.</span></span> |
| <span data-ttu-id="1b6d4-209">renderNoData</span><span class="sxs-lookup"><span data-stu-id="1b6d4-209">renderNoData</span></span> | <span data-ttu-id="1b6d4-210">Отрисовка пустого состояния данных.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-210">Renders an empty data state.</span></span> |
| <span data-ttu-id="1b6d4-211">renderGroups</span><span class="sxs-lookup"><span data-stu-id="1b6d4-211">renderGroups</span></span> | <span data-ttu-id="1b6d4-212">Сортировать данные событий по группам и отрисовки их с помощью заглавных групп.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-212">Sorts event data into groups and renders them with group headers.</span></span> |
| <span data-ttu-id="1b6d4-213">renderHeader</span><span class="sxs-lookup"><span data-stu-id="1b6d4-213">renderHeader</span></span> | <span data-ttu-id="1b6d4-214">Отрисовка загона группы.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-214">Renders a group header.</span></span> |
| <span data-ttu-id="1b6d4-215">renderEvents</span><span class="sxs-lookup"><span data-stu-id="1b6d4-215">renderEvents</span></span> | <span data-ttu-id="1b6d4-216">Отрисовка списка объектов событий.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-216">Renders a list of event objects.</span></span> |
| <span data-ttu-id="1b6d4-217">renderEvent</span><span class="sxs-lookup"><span data-stu-id="1b6d4-217">renderEvent</span></span> | <span data-ttu-id="1b6d4-218">Отрисовка события в единственном числе и всех его частей.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-218">Renders a singular event and all of its parts.</span></span>
| <span data-ttu-id="1b6d4-219">renderTitle</span><span class="sxs-lookup"><span data-stu-id="1b6d4-219">renderTitle</span></span> | <span data-ttu-id="1b6d4-220">Отрисовка части заголовка события.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-220">Renders the event title part.</span></span> |
| <span data-ttu-id="1b6d4-221">renderLocation</span><span class="sxs-lookup"><span data-stu-id="1b6d4-221">renderLocation</span></span> | <span data-ttu-id="1b6d4-222">Отрисовка части расположения события.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-222">Renders the event location part.</span></span> |
| <span data-ttu-id="1b6d4-223">renderAttendees</span><span class="sxs-lookup"><span data-stu-id="1b6d4-223">renderAttendees</span></span> | <span data-ttu-id="1b6d4-224">Отрисовка части участников события.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-224">Renders the event attendees part.</span></span> |
| <span data-ttu-id="1b6d4-225">renderOther</span><span class="sxs-lookup"><span data-stu-id="1b6d4-225">renderOther</span></span> | <span data-ttu-id="1b6d4-226">Отрисовка дополнительного содержимого события.</span><span class="sxs-lookup"><span data-stu-id="1b6d4-226">Renders additional event content.</span></span> |
