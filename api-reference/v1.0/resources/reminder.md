---
title: Тип ресурса reminder
description: Напоминание для события в календаре пользователя.
localization_priority: Normal
ms.openlocfilehash: e8aa591f078b90249b36d3dc2f666ddac4502461
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815724"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="9603d-103">Тип ресурса reminder</span><span class="sxs-lookup"><span data-stu-id="9603d-103">reminder resource type</span></span>

<span data-ttu-id="9603d-104">Напоминание для [события](event.md) в [Календарь](calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="9603d-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9603d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="9603d-105">Properties</span></span>
| <span data-ttu-id="9603d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="9603d-106">Property</span></span>     | <span data-ttu-id="9603d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="9603d-107">Type</span></span>   |<span data-ttu-id="9603d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9603d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9603d-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="9603d-109">changeKey</span></span>|<span data-ttu-id="9603d-110">String</span><span class="sxs-lookup"><span data-stu-id="9603d-110">String</span></span>|<span data-ttu-id="9603d-p101">Указывает версию напоминания. При каждом изменении напоминания также меняется значение **changeKey**. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="9603d-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="9603d-114">eventEndTime</span><span class="sxs-lookup"><span data-stu-id="9603d-114">eventEndTime</span></span>|[<span data-ttu-id="9603d-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9603d-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9603d-116">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="9603d-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="9603d-117">eventId</span><span class="sxs-lookup"><span data-stu-id="9603d-117">eventId</span></span>|<span data-ttu-id="9603d-118">String</span><span class="sxs-lookup"><span data-stu-id="9603d-118">String</span></span>|<span data-ttu-id="9603d-p102">Уникальный идентификатор события. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9603d-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="9603d-121">eventLocation</span><span class="sxs-lookup"><span data-stu-id="9603d-121">eventLocation</span></span>|[<span data-ttu-id="9603d-122">Location</span><span class="sxs-lookup"><span data-stu-id="9603d-122">Location</span></span>](location.md)|<span data-ttu-id="9603d-123">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="9603d-123">The location of the event.</span></span>|
|<span data-ttu-id="9603d-124">eventStartTime</span><span class="sxs-lookup"><span data-stu-id="9603d-124">eventStartTime</span></span>|[<span data-ttu-id="9603d-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9603d-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9603d-126">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="9603d-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="9603d-127">eventSubject</span><span class="sxs-lookup"><span data-stu-id="9603d-127">eventSubject</span></span>|<span data-ttu-id="9603d-128">String</span><span class="sxs-lookup"><span data-stu-id="9603d-128">String</span></span>|<span data-ttu-id="9603d-129">Текст в строке темы события.</span><span class="sxs-lookup"><span data-stu-id="9603d-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="9603d-130">eventWebLink</span><span class="sxs-lookup"><span data-stu-id="9603d-130">eventWebLink</span></span>|<span data-ttu-id="9603d-131">String</span><span class="sxs-lookup"><span data-stu-id="9603d-131">String</span></span>|<span data-ttu-id="9603d-132">URL-адрес для открытия события в Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="9603d-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="9603d-p103">Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.</span><span class="sxs-lookup"><span data-stu-id="9603d-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="9603d-135">Доступ к этому URL-адресу можно получить из объекта iFrame.</span><span class="sxs-lookup"><span data-stu-id="9603d-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="9603d-136">reminderFireTime</span><span class="sxs-lookup"><span data-stu-id="9603d-136">reminderFireTime</span></span>|[<span data-ttu-id="9603d-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9603d-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9603d-138">Дата, время и часовой пояс, заданные для упоминания.</span><span class="sxs-lookup"><span data-stu-id="9603d-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9603d-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9603d-139">JSON representation</span></span>

<span data-ttu-id="9603d-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9603d-140">Here is a JSON representation of the resource</span></span>

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
