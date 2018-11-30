---
title: Тип ресурса reminder
description: Напоминание для события в календаре пользователя.
ms.openlocfilehash: e7b7e2266b5959c6aa4927ecad52e24342d607e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078124"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="501fc-103">Тип ресурса reminder</span><span class="sxs-lookup"><span data-stu-id="501fc-103">reminder resource type</span></span>

> <span data-ttu-id="501fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="501fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="501fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="501fc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="501fc-106">Напоминание для [события](event.md) в [Календарь](calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="501fc-106">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="501fc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="501fc-107">Properties</span></span>
| <span data-ttu-id="501fc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="501fc-108">Property</span></span>     | <span data-ttu-id="501fc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="501fc-109">Type</span></span>   |<span data-ttu-id="501fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="501fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="501fc-111">changeKey</span><span class="sxs-lookup"><span data-stu-id="501fc-111">changeKey</span></span>|<span data-ttu-id="501fc-112">String</span><span class="sxs-lookup"><span data-stu-id="501fc-112">String</span></span>|<span data-ttu-id="501fc-p102">Указывает версию напоминания. При каждом изменении напоминания также меняется значение **changeKey**. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="501fc-p102">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="501fc-116">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="501fc-116">eventEndTime</span></span>|[<span data-ttu-id="501fc-117">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="501fc-117">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="501fc-118">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="501fc-118">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="501fc-119">eventId</span><span class="sxs-lookup"><span data-stu-id="501fc-119">eventId</span></span>|<span data-ttu-id="501fc-120">String</span><span class="sxs-lookup"><span data-stu-id="501fc-120">String</span></span>|<span data-ttu-id="501fc-p103">Уникальный идентификатор события. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="501fc-p103">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="501fc-123">eventLocation</span><span class="sxs-lookup"><span data-stu-id="501fc-123">eventLocation</span></span>|[<span data-ttu-id="501fc-124">Location</span><span class="sxs-lookup"><span data-stu-id="501fc-124">Location</span></span>](location.md)|<span data-ttu-id="501fc-125">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="501fc-125">The location of the event.</span></span>|
|<span data-ttu-id="501fc-126">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="501fc-126">eventStartTime</span></span>|[<span data-ttu-id="501fc-127">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="501fc-127">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="501fc-128">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="501fc-128">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="501fc-129">eventSubject</span><span class="sxs-lookup"><span data-stu-id="501fc-129">eventSubject</span></span>|<span data-ttu-id="501fc-130">String</span><span class="sxs-lookup"><span data-stu-id="501fc-130">String</span></span>|<span data-ttu-id="501fc-131">Текст в строке темы события.</span><span class="sxs-lookup"><span data-stu-id="501fc-131">The text of the event's subject line.</span></span>|
|<span data-ttu-id="501fc-132">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="501fc-132">eventWebLink</span></span>|<span data-ttu-id="501fc-133">String</span><span class="sxs-lookup"><span data-stu-id="501fc-133">String</span></span>|<span data-ttu-id="501fc-134">URL-адрес для открытия события в Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="501fc-134">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="501fc-p104">Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.</span><span class="sxs-lookup"><span data-stu-id="501fc-p104">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="501fc-137">Доступ к этому URL-адресу можно получить из объекта iFrame.</span><span class="sxs-lookup"><span data-stu-id="501fc-137">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="501fc-138">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="501fc-138">reminderFireTime</span></span>|[<span data-ttu-id="501fc-139">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="501fc-139">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="501fc-140">Дата, время и часовой пояс, заданные для упоминания.</span><span class="sxs-lookup"><span data-stu-id="501fc-140">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="501fc-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="501fc-141">JSON representation</span></span>

<span data-ttu-id="501fc-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="501fc-142">Here is a JSON representation of the resource</span></span>

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