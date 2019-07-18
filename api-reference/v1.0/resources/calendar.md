---
title: Тип ресурса calendar
description: Календарь, служащий контейнером для сведений о событиях. Это может быть календарь для пользователя или стандартный календарь для группы Office 365.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ab1d80073ea73b2e1b6321628218218f71d6ed24
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778343"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="5b911-104">Тип ресурса calendar</span><span class="sxs-lookup"><span data-stu-id="5b911-104">calendar resource type</span></span>

<span data-ttu-id="5b911-105">Календарь, служащий контейнером для сведений о событиях.</span><span class="sxs-lookup"><span data-stu-id="5b911-105">A calendar which is a container for events.</span></span> <span data-ttu-id="5b911-106">Это может быть календарь для ресурса [user](user.md) или стандартный календарь для ресурса [group](group.md), представляющего группу Office 365.</span><span class="sxs-lookup"><span data-stu-id="5b911-106">It can be a calendar for a [user](user.md), or the default calendar of an Office 365 [group](group.md).</span></span>

> <span data-ttu-id="5b911-107">**Примечание.** Существует несколько незначительных различий в способе взаимодействия с календарями пользователей и календарями групп:</span><span class="sxs-lookup"><span data-stu-id="5b911-107">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

- <span data-ttu-id="5b911-108">В ресурсе [calendarGroup](calendargroup.md) можно упорядочить только календари пользователей.</span><span class="sxs-lookup"><span data-stu-id="5b911-108">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="5b911-109">Outlook автоматически принимает все приглашения на собрания от имени группы.</span><span class="sxs-lookup"><span data-stu-id="5b911-109">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="5b911-110">Приглашения на собрания можно [принять](../api/event-accept.md), [принять под вопросом](../api/event-tentativelyaccept.md) или [отклонить](../api/event-decline.md) только в календарях пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b911-110">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
- <span data-ttu-id="5b911-111">Outlook не поддерживает напоминания о событиях группы.</span><span class="sxs-lookup"><span data-stu-id="5b911-111">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="5b911-112">[Напоминание](reminder.md) можно [отложить](../api/event-snoozereminder.md) или [отключить](../api/event-dismissreminder.md) только для календарей пользователя.</span><span class="sxs-lookup"><span data-stu-id="5b911-112">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="5b911-113">Методы</span><span class="sxs-lookup"><span data-stu-id="5b911-113">Methods</span></span>

| <span data-ttu-id="5b911-114">Метод</span><span class="sxs-lookup"><span data-stu-id="5b911-114">Method</span></span>       | <span data-ttu-id="5b911-115">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5b911-115">Return Type</span></span>  |<span data-ttu-id="5b911-116">Описание</span><span class="sxs-lookup"><span data-stu-id="5b911-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5b911-117">Список календарей</span><span class="sxs-lookup"><span data-stu-id="5b911-117">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="5b911-118">Коллекция [calendar](calendar.md)</span><span class="sxs-lookup"><span data-stu-id="5b911-118">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="5b911-119">Получение всех пользовательских календарей или календарей из стандартной либо другой указанной группы календарей.</span><span class="sxs-lookup"><span data-stu-id="5b911-119">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="5b911-120">Создание календаря</span><span class="sxs-lookup"><span data-stu-id="5b911-120">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="5b911-121">calendar</span><span class="sxs-lookup"><span data-stu-id="5b911-121">calendar</span></span>](calendar.md)| <span data-ttu-id="5b911-122">Создание календаря для пользователя в стандартной либо другой указанной группе календарей.</span><span class="sxs-lookup"><span data-stu-id="5b911-122">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="5b911-123">Получение календаря</span><span class="sxs-lookup"><span data-stu-id="5b911-123">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="5b911-124">calendar</span><span class="sxs-lookup"><span data-stu-id="5b911-124">calendar</span></span>](calendar.md) |<span data-ttu-id="5b911-125">Получение свойств и связей объекта **calendar**.</span><span class="sxs-lookup"><span data-stu-id="5b911-125">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="5b911-126">Это может быть календарь для пользователя или стандартный календарь для группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="5b911-126">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="5b911-127">Обновление</span><span class="sxs-lookup"><span data-stu-id="5b911-127">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="5b911-128">calendar</span><span class="sxs-lookup"><span data-stu-id="5b911-128">calendar</span></span>](calendar.md)  |<span data-ttu-id="5b911-129">Обновление свойств объекта **calendar**.</span><span class="sxs-lookup"><span data-stu-id="5b911-129">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="5b911-130">Это может быть календарь для пользователя или стандартный календарь для группы Office 365.</span><span class="sxs-lookup"><span data-stu-id="5b911-130">The calendar can be one for a user, or the default calendar of an Office 365 group.</span></span> |
|[<span data-ttu-id="5b911-131">Удаление</span><span class="sxs-lookup"><span data-stu-id="5b911-131">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="5b911-132">Нет</span><span class="sxs-lookup"><span data-stu-id="5b911-132">None</span></span> |<span data-ttu-id="5b911-133">Удаление объекта calendar.</span><span class="sxs-lookup"><span data-stu-id="5b911-133">Delete calendar object.</span></span> |
|[<span data-ttu-id="5b911-134">Список экземпляров calendarView</span><span class="sxs-lookup"><span data-stu-id="5b911-134">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="5b911-135">Коллекция [event](event.md)</span><span class="sxs-lookup"><span data-stu-id="5b911-135">[event](event.md) collection</span></span>| <span data-ttu-id="5b911-136">Получение в представлении календаря повторений, исключений и отдельных экземпляров событий за определенный диапазон времени, указанных в основном календаре пользователя `(../me/calendarview)` или в другом заданном календаре.</span><span class="sxs-lookup"><span data-stu-id="5b911-136">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="5b911-137">Список событий</span><span class="sxs-lookup"><span data-stu-id="5b911-137">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="5b911-138">Коллекция [event](event.md)</span><span class="sxs-lookup"><span data-stu-id="5b911-138">[event](event.md) collection</span></span>| <span data-ttu-id="5b911-p107">Получение списка событий в календаре. Этот список содержит собрания с одним экземпляром и образцы рядов.</span><span class="sxs-lookup"><span data-stu-id="5b911-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="5b911-141">Создание события</span><span class="sxs-lookup"><span data-stu-id="5b911-141">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="5b911-142">event</span><span class="sxs-lookup"><span data-stu-id="5b911-142">event</span></span>](event.md)| <span data-ttu-id="5b911-143">Создание события в стандартном или указанном календаре.</span><span class="sxs-lookup"><span data-stu-id="5b911-143">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="5b911-144">getSchedule</span><span class="sxs-lookup"><span data-stu-id="5b911-144">getSchedule</span></span>](../api/calendar-getschedule.md) |<span data-ttu-id="5b911-145">Коллекция [scheduleInformation](scheduleinformation.md)</span><span class="sxs-lookup"><span data-stu-id="5b911-145">[scheduleInformation](scheduleinformation.md) collection</span></span>|<span data-ttu-id="5b911-146">Получение сведений о доступности коллекции пользователей, списков рассылки или ресурсов для определенного периода времени.</span><span class="sxs-lookup"><span data-stu-id="5b911-146">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span> |
|[<span data-ttu-id="5b911-147">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="5b911-147">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="5b911-148">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="5b911-148">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="5b911-149">Предложение времени проведения собрания и местоположения с учетом доступности организатора и участников, а также ограничений по местоположению или времени.</span><span class="sxs-lookup"><span data-stu-id="5b911-149">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="5b911-150">Создание однозначного расширенного свойства</span><span class="sxs-lookup"><span data-stu-id="5b911-150">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="5b911-151">calendar</span><span class="sxs-lookup"><span data-stu-id="5b911-151">calendar</span></span>](calendar.md)  |<span data-ttu-id="5b911-152">Создание одного или нескольких расширенных свойств с одним значением в новом или существующем календаре.</span><span class="sxs-lookup"><span data-stu-id="5b911-152">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="5b911-153">Получение календаря с расширенным свойством с одним значением</span><span class="sxs-lookup"><span data-stu-id="5b911-153">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="5b911-154">calendar</span><span class="sxs-lookup"><span data-stu-id="5b911-154">calendar</span></span>](calendar.md) | <span data-ttu-id="5b911-155">Получение календарей, которые содержат расширенное свойство с одним значением, при помощи `$expand` или `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5b911-155">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="5b911-156">Создание расширенного свойства с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="5b911-156">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="5b911-157">calendar</span><span class="sxs-lookup"><span data-stu-id="5b911-157">calendar</span></span>](calendar.md) | <span data-ttu-id="5b911-158">Создание одного или нескольких расширенных свойств с несколькими значениями в новом или существующем календаре.</span><span class="sxs-lookup"><span data-stu-id="5b911-158">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="5b911-159">Получение календаря с расширенным свойством с несколькими значениями</span><span class="sxs-lookup"><span data-stu-id="5b911-159">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="5b911-160">calendar</span><span class="sxs-lookup"><span data-stu-id="5b911-160">calendar</span></span>](calendar.md) | <span data-ttu-id="5b911-161">Получение календаря, который содержит расширенное свойство с несколькими значениями, при помощи `$expand`.</span><span class="sxs-lookup"><span data-stu-id="5b911-161">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="5b911-162">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b911-162">Properties</span></span>
| <span data-ttu-id="5b911-163">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b911-163">Property</span></span>     | <span data-ttu-id="5b911-164">Тип</span><span class="sxs-lookup"><span data-stu-id="5b911-164">Type</span></span>   |<span data-ttu-id="5b911-165">Описание</span><span class="sxs-lookup"><span data-stu-id="5b911-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b911-166">canEdit</span><span class="sxs-lookup"><span data-stu-id="5b911-166">canEdit</span></span> |<span data-ttu-id="5b911-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b911-167">Boolean</span></span> |<span data-ttu-id="5b911-p108">Значение true, если пользователь может вносить изменения в календарь, в противном случае — значение false. Это свойство имеет значение true для пользователя, создавшего календарь. Это свойство также имеет значение true для пользователей, которые совместно используют календарь и имеют доступ на запись.</span><span class="sxs-lookup"><span data-stu-id="5b911-p108">True if the user can write to the calendar, false otherwise. This property is true for the user who created the calendar. This property is also true for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="5b911-171">canShare</span><span class="sxs-lookup"><span data-stu-id="5b911-171">canShare</span></span> |<span data-ttu-id="5b911-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b911-172">Boolean</span></span> |<span data-ttu-id="5b911-p109">Значение true, если у пользователя есть разрешение на совместное использование календаря, в противном случае — значение false. Только пользователь, создавший календарь, может предоставлять общий доступ к нему.</span><span class="sxs-lookup"><span data-stu-id="5b911-p109">True if the user has the permission to share the calendar, false otherwise. Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="5b911-175">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="5b911-175">canViewPrivateItems</span></span> |<span data-ttu-id="5b911-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="5b911-176">Boolean</span></span> |<span data-ttu-id="5b911-177">Значение true, если пользователь может читать элементы календаря, которые были помечены как частные, в противном случае — значение false.</span><span class="sxs-lookup"><span data-stu-id="5b911-177">True if the user can read calendar items that have been marked private, false otherwise.</span></span> |
|<span data-ttu-id="5b911-178">changeKey</span><span class="sxs-lookup"><span data-stu-id="5b911-178">changeKey</span></span>|<span data-ttu-id="5b911-179">String</span><span class="sxs-lookup"><span data-stu-id="5b911-179">String</span></span>|<span data-ttu-id="5b911-p110">Указывает версию объекта calendar. При каждом изменении календаря также меняется значение changeKey. Благодаря этому Exchange может применять изменения к правильной версии объекта. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b911-p110">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="5b911-184">color</span><span class="sxs-lookup"><span data-stu-id="5b911-184">color</span></span>|<span data-ttu-id="5b911-185">calendarColor</span><span class="sxs-lookup"><span data-stu-id="5b911-185">calendarColor</span></span>|<span data-ttu-id="5b911-p111">Задает цветовую тему, отличающую этот календарь от других календарей в пользовательском интерфейсе. Значения свойств: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span><span class="sxs-lookup"><span data-stu-id="5b911-p111">Specifies the color theme to distinguish the calendar from other calendars in a UI. The property values are: LightBlue=0, LightGreen=1, LightOrange=2, LightGray=3, LightYellow=4, LightTeal=5, LightPink=6, LightBrown=7, LightRed=8, MaxColor=9, Auto=-1</span></span>|
|<span data-ttu-id="5b911-188">id</span><span class="sxs-lookup"><span data-stu-id="5b911-188">id</span></span>|<span data-ttu-id="5b911-189">Строка</span><span class="sxs-lookup"><span data-stu-id="5b911-189">String</span></span>|<span data-ttu-id="5b911-p112">Уникальный идентификатор группы. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b911-p112">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="5b911-192">имя</span><span class="sxs-lookup"><span data-stu-id="5b911-192">name</span></span>|<span data-ttu-id="5b911-193">String</span><span class="sxs-lookup"><span data-stu-id="5b911-193">String</span></span>|<span data-ttu-id="5b911-194">Имя календаря.</span><span class="sxs-lookup"><span data-stu-id="5b911-194">The calendar name.</span></span>|
|<span data-ttu-id="5b911-195">owner</span><span class="sxs-lookup"><span data-stu-id="5b911-195">owner</span></span> |[<span data-ttu-id="5b911-196">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5b911-196">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="5b911-p113">Если это свойство задано, оно указывает на пользователя, создавшего или добавившего календарь. В календаре, созданном или добавленном пользователем, свойство **owner** установлено для этого пользователя. В календаре, который используется совместно с пользователем, свойство **owner** установлено для лица, предоставившего пользователю общий доступ к этому календарю.</span><span class="sxs-lookup"><span data-stu-id="5b911-p113">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5b911-200">Связи</span><span class="sxs-lookup"><span data-stu-id="5b911-200">Relationships</span></span>
| <span data-ttu-id="5b911-201">Отношение</span><span class="sxs-lookup"><span data-stu-id="5b911-201">Relationship</span></span> | <span data-ttu-id="5b911-202">Тип</span><span class="sxs-lookup"><span data-stu-id="5b911-202">Type</span></span>   |<span data-ttu-id="5b911-203">Описание</span><span class="sxs-lookup"><span data-stu-id="5b911-203">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b911-204">calendarView</span><span class="sxs-lookup"><span data-stu-id="5b911-204">calendarView</span></span>|<span data-ttu-id="5b911-205">Коллекция [Event](event.md)</span><span class="sxs-lookup"><span data-stu-id="5b911-205">[Event](event.md) collection</span></span>|<span data-ttu-id="5b911-p114">Представление календаря для календаря. Свойство навигации. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b911-p114">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="5b911-209">события</span><span class="sxs-lookup"><span data-stu-id="5b911-209">events</span></span>|<span data-ttu-id="5b911-210">Коллекция [Event](event.md)</span><span class="sxs-lookup"><span data-stu-id="5b911-210">[Event](event.md) collection</span></span>|<span data-ttu-id="5b911-p115">События в календаре. Свойство навигации. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5b911-p115">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="5b911-214">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5b911-214">multiValueExtendedProperties</span></span>|<span data-ttu-id="5b911-215">Коллекция [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5b911-215">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5b911-p116">Коллекция расширенных свойств с несколькими значениями, определенных для календаря. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5b911-p116">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="5b911-219">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="5b911-219">singleValueExtendedProperties</span></span>|<span data-ttu-id="5b911-220">Коллекция [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)</span><span class="sxs-lookup"><span data-stu-id="5b911-220">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="5b911-p117">Коллекция расширенных свойств с одним значением, определенных для календаря. Только для чтения. Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="5b911-p117">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b911-224">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b911-224">JSON representation</span></span>

<span data-ttu-id="5b911-225">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b911-225">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "id": "string (identifier)",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
