---
title: Компонент повестки в наборе инструментов Microsoft Graph
description: Веб-компонент "центр центровой связи" используется для представления событий в календаре пользователя или группы.
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: c42b62241f5eee7fef51bf57bf8617dd6e89b8c6
ms.sourcegitcommit: 566d09c17f9d641b6fac9b9159405a3cc41e037b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/20/2020
ms.locfileid: "45183927"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="8894b-103">Компонент повестки в наборе инструментов Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8894b-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="8894b-104">`mgt-agenda`Веб-компонент представляет события в календаре пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="8894b-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="8894b-105">По умолчанию в календаре отображаются текущие события пользователя, вошедшего в текущий день.</span><span class="sxs-lookup"><span data-stu-id="8894b-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="8894b-106">Компонент также может использовать любую конечную точку, возвращающую события из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8894b-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span>

## <a name="example"></a><span data-ttu-id="8894b-107">Пример</span><span class="sxs-lookup"><span data-stu-id="8894b-107">Example</span></span>

<span data-ttu-id="8894b-108">В следующем примере показаны события календаря вошедшего пользователя, отображаемые с помощью `mgt-agenda` компонента.</span><span class="sxs-lookup"><span data-stu-id="8894b-108">The following example shows the signed-in user's calendar events displayed using the `mgt-agenda` component.</span></span> <span data-ttu-id="8894b-109">С помощью редактора кода можно увидеть, как [Свойства](#properties) изменяют поведение компонента.</span><span class="sxs-lookup"><span data-stu-id="8894b-109">You can use the code editor to see how [properties](#properties) change the behavior of the component.</span></span>

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-agenda--simple&source=docs" height="500"></iframe>

[<span data-ttu-id="8894b-110">Откройте этот пример в меню упр. dev.</span><span class="sxs-lookup"><span data-stu-id="8894b-110">Open this example in mgt.dev</span></span>](https://mgt.dev/?path=/story/components-mgt-agenda--simple&source=docs)

## <a name="properties"></a><span data-ttu-id="8894b-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="8894b-111">Properties</span></span>

<span data-ttu-id="8894b-112">По умолчанию `mgt-agenda` компонент получает события от `/me/calendarview` конечной точки и отображает события за текущий день.</span><span class="sxs-lookup"><span data-stu-id="8894b-112">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="8894b-113">Существует несколько свойств, которые можно использовать для изменения этого поведения.</span><span class="sxs-lookup"><span data-stu-id="8894b-113">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="8894b-114">Атрибут</span><span class="sxs-lookup"><span data-stu-id="8894b-114">Attribute</span></span> | <span data-ttu-id="8894b-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="8894b-115">Property</span></span> | <span data-ttu-id="8894b-116">Описание</span><span class="sxs-lookup"><span data-stu-id="8894b-116">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="8894b-117">дата</span><span class="sxs-lookup"><span data-stu-id="8894b-117">date</span></span> | <span data-ttu-id="8894b-118">date</span><span class="sxs-lookup"><span data-stu-id="8894b-118">date</span></span> | <span data-ttu-id="8894b-119">Строка, представляющая дату начала событий, которые необходимо получить из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8894b-119">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="8894b-120">Значение должно быть в формате, который может быть проанализирован с помощью [конструктора Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -value, если `event-query` задан атрибут.</span><span class="sxs-lookup"><span data-stu-id="8894b-120">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="8894b-121">срок</span><span class="sxs-lookup"><span data-stu-id="8894b-121">days</span></span> | <span data-ttu-id="8894b-122">срок</span><span class="sxs-lookup"><span data-stu-id="8894b-122">days</span></span> | <span data-ttu-id="8894b-123">Число дней для выборки из Microsoft Graph — значение по умолчанию не оказывает никакого действия, если `event-query` задан атрибут.</span><span class="sxs-lookup"><span data-stu-id="8894b-123">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| <span data-ttu-id="8894b-124">Show — Max</span><span class="sxs-lookup"><span data-stu-id="8894b-124">show-max</span></span> | <span data-ttu-id="8894b-125">шовмакс</span><span class="sxs-lookup"><span data-stu-id="8894b-125">showMax</span></span> | <span data-ttu-id="8894b-126">Число, определяющее максимальное число отображаемых событий.</span><span class="sxs-lookup"><span data-stu-id="8894b-126">A number to indicate the maximum number of events to show.</span></span> <span data-ttu-id="8894b-127">Значение по умолчанию не задано (максимальное значение не задано).</span><span class="sxs-lookup"><span data-stu-id="8894b-127">The default value is not set (no maximum).</span></span> |
| <span data-ttu-id="8894b-128">Идентификатор группы</span><span class="sxs-lookup"><span data-stu-id="8894b-128">group-id</span></span> | <span data-ttu-id="8894b-129">groupId</span><span class="sxs-lookup"><span data-stu-id="8894b-129">groupId</span></span> | <span data-ttu-id="8894b-130">Идентификатор строки для календаря группы, который будет использоваться вместо текущего календаря пользователя, выполнившего вход.</span><span class="sxs-lookup"><span data-stu-id="8894b-130">A string ID for a group calendar to use instead of the current signed in user's calendar.</span></span> |
| <span data-ttu-id="8894b-131">событие — запрос</span><span class="sxs-lookup"><span data-stu-id="8894b-131">event-query</span></span> | <span data-ttu-id="8894b-132">евенткуери</span><span class="sxs-lookup"><span data-stu-id="8894b-132">eventQuery</span></span> | <span data-ttu-id="8894b-133">Строка, представляющая альтернативный запрос, который будет использоваться при получении событий из Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="8894b-133">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="8894b-134">При необходимости добавьте делегированную область в конец строки, чтобы она была ограничена `|` ( `/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all` ).</span><span class="sxs-lookup"><span data-stu-id="8894b-134">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all`).</span></span> |
| <span data-ttu-id="8894b-135">events</span><span class="sxs-lookup"><span data-stu-id="8894b-135">events</span></span> | <span data-ttu-id="8894b-136">events</span><span class="sxs-lookup"><span data-stu-id="8894b-136">events</span></span> | <span data-ttu-id="8894b-137">Массив событий, чтобы получить или задать список событий, отображаемых компонентом, с помощью этого свойства можно получить доступ к событиям, загруженным компонентом.</span><span class="sxs-lookup"><span data-stu-id="8894b-137">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="8894b-138">Присвойте этому значению значение загрузка собственных событий, если значение задано разработчиком, `date` `days` атрибуты, или, атрибуты, `event-query` не действуют.</span><span class="sxs-lookup"><span data-stu-id="8894b-138">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |
| <span data-ttu-id="8894b-139">Группировка по дням</span><span class="sxs-lookup"><span data-stu-id="8894b-139">group-by-day</span></span> | <span data-ttu-id="8894b-140">граупбидай</span><span class="sxs-lookup"><span data-stu-id="8894b-140">groupByDay</span></span> | <span data-ttu-id="8894b-141">Логическое значение для группировки событий по дням события по умолчанию не группируются.</span><span class="sxs-lookup"><span data-stu-id="8894b-141">A Boolean value to group events by day - by default events are not grouped.</span></span> |

<span data-ttu-id="8894b-142">В следующем примере показано, как изменить поведение компонента для извлечения данных за определенную дату и до трех дней.</span><span class="sxs-lookup"><span data-stu-id="8894b-142">The following example changes the behavior of the component to fetch data for a specific date and up to three days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="8894b-143">В следующем примере показано изменение поведения компонента для извлечения данных из определенного запроса.</span><span class="sxs-lookup"><span data-stu-id="8894b-143">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="8894b-144">Настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="8894b-144">CSS custom properties</span></span>

<span data-ttu-id="8894b-145">`mgt-agenda`Компонент определяет следующие настраиваемые свойства CSS</span><span class="sxs-lookup"><span data-stu-id="8894b-145">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="8894b-146">Чтобы узнать больше, ознакомьтесь с разделами [стилизация компонентов](../style.md).</span><span class="sxs-lookup"><span data-stu-id="8894b-146">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="8894b-147">Шаблоны</span><span class="sxs-lookup"><span data-stu-id="8894b-147">Templates</span></span>

<span data-ttu-id="8894b-148">`mgt-agenda`Компонент поддерживает несколько [шаблонов](../templates.md) , позволяющих заменить определенные части компонента.</span><span class="sxs-lookup"><span data-stu-id="8894b-148">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="8894b-149">Чтобы указать шаблон, включите элемент в `<template>` компонент и задайте `data-type` для него одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="8894b-149">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="8894b-150">Тип данных</span><span class="sxs-lookup"><span data-stu-id="8894b-150">Data type</span></span> | <span data-ttu-id="8894b-151">Контекст данных</span><span class="sxs-lookup"><span data-stu-id="8894b-151">Data context</span></span> | <span data-ttu-id="8894b-152">Описание</span><span class="sxs-lookup"><span data-stu-id="8894b-152">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="8894b-153">`events`: список объектов Event</span><span class="sxs-lookup"><span data-stu-id="8894b-153">`events`: list of event objects</span></span> | <span data-ttu-id="8894b-154">Шаблон по умолчанию заменяет весь компонент своим собственным.</span><span class="sxs-lookup"><span data-stu-id="8894b-154">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="8894b-155">`event`: объект Event</span><span class="sxs-lookup"><span data-stu-id="8894b-155">`event`: event object</span></span> | <span data-ttu-id="8894b-156">Шаблон, используемый для отображения каждого события.</span><span class="sxs-lookup"><span data-stu-id="8894b-156">The template used to render each event.</span></span> |
| `event-other` | <span data-ttu-id="8894b-157">`event`: объект Event</span><span class="sxs-lookup"><span data-stu-id="8894b-157">`event`: event object</span></span> | <span data-ttu-id="8894b-158">Шаблон, используемый для отображения дополнительного содержимого для каждого события.</span><span class="sxs-lookup"><span data-stu-id="8894b-158">The template used to render additional content for each event.</span></span> |
| `header` | <span data-ttu-id="8894b-159">`header`: строка</span><span class="sxs-lookup"><span data-stu-id="8894b-159">`header`: string</span></span> | <span data-ttu-id="8894b-160">Шаблон, используемый для отображения заголовка ежедневно.</span><span class="sxs-lookup"><span data-stu-id="8894b-160">The template used to render the header for each day.</span></span> |
| `loading` | <span data-ttu-id="8894b-161">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="8894b-161">No data context is passed</span></span> | <span data-ttu-id="8894b-162">Шаблон, используемый при загрузке данных.</span><span class="sxs-lookup"><span data-stu-id="8894b-162">The template used when data is loading.</span></span> |
| `no-data` | <span data-ttu-id="8894b-163">Контекст данных не передается</span><span class="sxs-lookup"><span data-stu-id="8894b-163">No data context is passed</span></span> | <span data-ttu-id="8894b-164">Шаблон, используемый при отсутствии доступных событий.</span><span class="sxs-lookup"><span data-stu-id="8894b-164">The template used when no events are available.</span></span> |

<span data-ttu-id="8894b-165">В следующих примерах показано, как использовать `event` шаблон:</span><span class="sxs-lookup"><span data-stu-id="8894b-165">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="8894b-166">Чтобы узнать больше, ознакомьтесь со статьей [шаблоны](../templates.md).</span><span class="sxs-lookup"><span data-stu-id="8894b-166">To learn more, see [templates](../templates.md).</span></span>

## <a name="events"></a><span data-ttu-id="8894b-167">События</span><span class="sxs-lookup"><span data-stu-id="8894b-167">Events</span></span>

<span data-ttu-id="8894b-168">Из элемента управления запускаются следующие события.</span><span class="sxs-lookup"><span data-stu-id="8894b-168">The following events are fired from the control.</span></span>

| <span data-ttu-id="8894b-169">Событие</span><span class="sxs-lookup"><span data-stu-id="8894b-169">Event</span></span> | <span data-ttu-id="8894b-170">Описание</span><span class="sxs-lookup"><span data-stu-id="8894b-170">Description</span></span> |
| --- | --- |
| <span data-ttu-id="8894b-171">евенткликк</span><span class="sxs-lookup"><span data-stu-id="8894b-171">eventClick</span></span> | <span data-ttu-id="8894b-172">Пользователь щелкает или отменяет событие.</span><span class="sxs-lookup"><span data-stu-id="8894b-172">The user clicks or taps an event.</span></span>|

## <a name="permissions"></a><span data-ttu-id="8894b-173">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8894b-173">Permissions</span></span>

<span data-ttu-id="8894b-174">В этом компоненте используются следующие API и разрешения Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="8894b-174">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="8894b-175">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8894b-175">Resource</span></span> | <span data-ttu-id="8894b-176">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8894b-176">Permission</span></span> |
| - | - |
| [<span data-ttu-id="8894b-177">/ме/календарвиев</span><span class="sxs-lookup"><span data-stu-id="8894b-177">/me/calendarview</span></span>](/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | <span data-ttu-id="8894b-178">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="8894b-178">Calendars.Read</span></span> |

<span data-ttu-id="8894b-179">Компонент позволяет указать другой запрос Microsoft Graph для вызова (например, `/groups/{id}/calendar/calendarView` ).</span><span class="sxs-lookup"><span data-stu-id="8894b-179">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="8894b-180">В этом случае необходимо добавить разрешение в конец строки, с разделителем `|` .</span><span class="sxs-lookup"><span data-stu-id="8894b-180">In this case, append the permission to the end of the string, delimited by `|`.</span></span>

<span data-ttu-id="8894b-181">При использовании шаблона по умолчанию и шаблона по умолчанию `renderAttendees` требуются дополнительные API и разрешения.</span><span class="sxs-lookup"><span data-stu-id="8894b-181">When using the default template and default `renderAttendees` template, additional APIs and permissions are required.</span></span> <span data-ttu-id="8894b-182">В шаблоне по умолчанию для этого компонента используется компонент [упр. People](people.md) для событий, которые содержат участников, для которых требуется следующее.</span><span class="sxs-lookup"><span data-stu-id="8894b-182">The default template for this component uses a [mgt-people](people.md) component for events that have attendees, which requires the following.</span></span>

| <span data-ttu-id="8894b-183">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8894b-183">Resource</span></span> | <span data-ttu-id="8894b-184">Разрешение</span><span class="sxs-lookup"><span data-stu-id="8894b-184">Permission</span></span> |
| - | - |
| [<span data-ttu-id="8894b-185">/Users</span><span class="sxs-lookup"><span data-stu-id="8894b-185">/users</span></span>](/graph/api/user-list?view=graph-rest-1.0) | <span data-ttu-id="8894b-186">Users. ReadBasic. ALL</span><span class="sxs-lookup"><span data-stu-id="8894b-186">Users.ReadBasic.All</span></span> |
| [<span data-ttu-id="8894b-187">/ме/календарвиев</span><span class="sxs-lookup"><span data-stu-id="8894b-187">/me/calendarview</span></span>](/graph/api/user-list-people?view=graph-rest-1.0) | <span data-ttu-id="8894b-188">People.Read</span><span class="sxs-lookup"><span data-stu-id="8894b-188">People.Read</span></span> |
| [<span data-ttu-id="8894b-189">/ме/календарвиев</span><span class="sxs-lookup"><span data-stu-id="8894b-189">/me/calendarview</span></span>](/graph/api/user-list-contacts?view=graph-rest-1.0) | <span data-ttu-id="8894b-190">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="8894b-190">Contacts.Read</span></span> |

## <a name="authentication"></a><span data-ttu-id="8894b-191">Проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="8894b-191">Authentication</span></span>

<span data-ttu-id="8894b-192">Элемент управления входом использует глобальную службу проверки подлинности, описанную в [документации по проверке подлинности](./../providers.md).</span><span class="sxs-lookup"><span data-stu-id="8894b-192">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span>

## <a name="extend-for-more-control"></a><span data-ttu-id="8894b-193">Расширение для дополнительных элементов управления</span><span class="sxs-lookup"><span data-stu-id="8894b-193">Extend for more control</span></span>

<span data-ttu-id="8894b-194">Для более сложных сценариев или для действительно настраиваемого пользовательского интерфейса этот компонент предоставляет несколько `protected` методов Render \* для переопределения в расширениях компонентов.</span><span class="sxs-lookup"><span data-stu-id="8894b-194">For more complex scenarios or a truly custom UX, this component exposes several `protected` render\* methods for override in component extensions.</span></span>

| <span data-ttu-id="8894b-195">Метод</span><span class="sxs-lookup"><span data-stu-id="8894b-195">Method</span></span> | <span data-ttu-id="8894b-196">Описание</span><span class="sxs-lookup"><span data-stu-id="8894b-196">Description</span></span> |
| - | - |
| <span data-ttu-id="8894b-197">рендерлоадинг</span><span class="sxs-lookup"><span data-stu-id="8894b-197">renderLoading</span></span> | <span data-ttu-id="8894b-198">Отображает состояние загрузки при загрузке компонента.</span><span class="sxs-lookup"><span data-stu-id="8894b-198">Renders a loading state while the component loads.</span></span> |
| <span data-ttu-id="8894b-199">рендернодата</span><span class="sxs-lookup"><span data-stu-id="8894b-199">renderNoData</span></span> | <span data-ttu-id="8894b-200">Отрисовывает пустое состояние данных.</span><span class="sxs-lookup"><span data-stu-id="8894b-200">Renders an empty data state.</span></span> |
| <span data-ttu-id="8894b-201">рендерграупс</span><span class="sxs-lookup"><span data-stu-id="8894b-201">renderGroups</span></span> | <span data-ttu-id="8894b-202">Сортирует данные события по группам и отображает их с помощью заголовков групп.</span><span class="sxs-lookup"><span data-stu-id="8894b-202">Sorts event data into groups and renders them with group headers.</span></span> |
| <span data-ttu-id="8894b-203">рендерхеадер</span><span class="sxs-lookup"><span data-stu-id="8894b-203">renderHeader</span></span> | <span data-ttu-id="8894b-204">Отрисовывает заголовок группы.</span><span class="sxs-lookup"><span data-stu-id="8894b-204">Renders a group header.</span></span> |
| <span data-ttu-id="8894b-205">рендеревентс</span><span class="sxs-lookup"><span data-stu-id="8894b-205">renderEvents</span></span> | <span data-ttu-id="8894b-206">Отрисовывает список объектов Event.</span><span class="sxs-lookup"><span data-stu-id="8894b-206">Renders a list of event objects.</span></span> |
| <span data-ttu-id="8894b-207">рендеревент</span><span class="sxs-lookup"><span data-stu-id="8894b-207">renderEvent</span></span> | <span data-ttu-id="8894b-208">Отображает единственное событие и все его части.</span><span class="sxs-lookup"><span data-stu-id="8894b-208">Renders a singular event and all of its parts.</span></span>
| <span data-ttu-id="8894b-209">рендертитле</span><span class="sxs-lookup"><span data-stu-id="8894b-209">renderTitle</span></span> | <span data-ttu-id="8894b-210">Отрисовывает часть заголовка события.</span><span class="sxs-lookup"><span data-stu-id="8894b-210">Renders the event title part.</span></span> |
| <span data-ttu-id="8894b-211">рендерлокатион</span><span class="sxs-lookup"><span data-stu-id="8894b-211">renderLocation</span></span> | <span data-ttu-id="8894b-212">Отрисовывает часть расположения события.</span><span class="sxs-lookup"><span data-stu-id="8894b-212">Renders the event location part.</span></span> |
| <span data-ttu-id="8894b-213">рендераттендис</span><span class="sxs-lookup"><span data-stu-id="8894b-213">renderAttendees</span></span> | <span data-ttu-id="8894b-214">Отрисовывает часть участников события.</span><span class="sxs-lookup"><span data-stu-id="8894b-214">Renders the event attendees part.</span></span> |
| <span data-ttu-id="8894b-215">рендеросер</span><span class="sxs-lookup"><span data-stu-id="8894b-215">renderOther</span></span> | <span data-ttu-id="8894b-216">Отображает дополнительный контент события.</span><span class="sxs-lookup"><span data-stu-id="8894b-216">Renders additional event content.</span></span> |
