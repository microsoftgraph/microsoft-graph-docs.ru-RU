---
title: Тип ресурса reminder
description: Напоминание для события в календаре пользователя.
localization_priority: Normal
ms.openlocfilehash: a78c7f82ea0a7db9da45a60de98bb3b1311aaeeb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819966"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="89718-103">Тип ресурса reminder</span><span class="sxs-lookup"><span data-stu-id="89718-103">reminder resource type</span></span>

> <span data-ttu-id="89718-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="89718-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89718-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89718-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89718-106">Напоминание для [события](event.md) в [Календарь](calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="89718-106">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="89718-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="89718-107">Properties</span></span>
| <span data-ttu-id="89718-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="89718-108">Property</span></span>     | <span data-ttu-id="89718-109">Тип</span><span class="sxs-lookup"><span data-stu-id="89718-109">Type</span></span>   |<span data-ttu-id="89718-110">Описание</span><span class="sxs-lookup"><span data-stu-id="89718-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89718-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="89718-111">changeKey</span></span>|<span data-ttu-id="89718-112">String</span><span class="sxs-lookup"><span data-stu-id="89718-112">String</span></span>|<span data-ttu-id="89718-p102">Указывает версию напоминания. При каждом изменении напоминания также меняется значение **changeKey**. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="89718-p102">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="89718-116">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="89718-116">eventEndTime</span></span>|[<span data-ttu-id="89718-117">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="89718-117">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="89718-118">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="89718-118">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="89718-119">eventId</span><span class="sxs-lookup"><span data-stu-id="89718-119">eventId</span></span>|<span data-ttu-id="89718-120">String</span><span class="sxs-lookup"><span data-stu-id="89718-120">String</span></span>|<span data-ttu-id="89718-p103">Уникальный идентификатор события. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="89718-p103">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="89718-123">eventLocation</span><span class="sxs-lookup"><span data-stu-id="89718-123">eventLocation</span></span>|[<span data-ttu-id="89718-124">Location</span><span class="sxs-lookup"><span data-stu-id="89718-124">Location</span></span>](location.md)|<span data-ttu-id="89718-125">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="89718-125">The location of the event.</span></span>|
|<span data-ttu-id="89718-126">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="89718-126">eventStartTime</span></span>|[<span data-ttu-id="89718-127">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="89718-127">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="89718-128">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="89718-128">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="89718-129">eventSubject</span><span class="sxs-lookup"><span data-stu-id="89718-129">eventSubject</span></span>|<span data-ttu-id="89718-130">String</span><span class="sxs-lookup"><span data-stu-id="89718-130">String</span></span>|<span data-ttu-id="89718-131">Текст в строке темы события.</span><span class="sxs-lookup"><span data-stu-id="89718-131">The text of the event's subject line.</span></span>|
|<span data-ttu-id="89718-132">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="89718-132">eventWebLink</span></span>|<span data-ttu-id="89718-133">String</span><span class="sxs-lookup"><span data-stu-id="89718-133">String</span></span>|<span data-ttu-id="89718-134">URL-адрес для открытия события в Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="89718-134">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="89718-p104">Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.</span><span class="sxs-lookup"><span data-stu-id="89718-p104">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="89718-137">Доступ к этому URL-адресу можно получить из объекта iFrame.</span><span class="sxs-lookup"><span data-stu-id="89718-137">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="89718-138">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="89718-138">reminderFireTime</span></span>|[<span data-ttu-id="89718-139">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="89718-139">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="89718-140">Дата, время и часовой пояс, заданные для упоминания.</span><span class="sxs-lookup"><span data-stu-id="89718-140">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89718-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89718-141">JSON representation</span></span>

<span data-ttu-id="89718-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89718-142">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.reminder"
}-->

```json
{
  "changeKey": "string",
  "eventEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventId": "string",
  "eventLocation": {"@odata.type": "microsoft.graph.location"},
  "eventStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "eventSubject": "string",
  "eventWebLink": "string",
  "reminderFireTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
