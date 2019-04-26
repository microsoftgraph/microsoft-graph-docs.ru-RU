---
title: Тип ресурса reminder
description: Напоминание о событии в календаре пользователя.
localization_priority: Normal
ms.openlocfilehash: b68e0553bcee946fe32146bc15151f6ed97163cd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343866"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="b249e-103">Тип ресурса reminder</span><span class="sxs-lookup"><span data-stu-id="b249e-103">reminder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b249e-104">Напоминание о [событии](event.md) в календаре [](calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="b249e-104">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b249e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b249e-105">Properties</span></span>
| <span data-ttu-id="b249e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b249e-106">Property</span></span>     | <span data-ttu-id="b249e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b249e-107">Type</span></span>   |<span data-ttu-id="b249e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b249e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b249e-109">changeKey</span><span class="sxs-lookup"><span data-stu-id="b249e-109">changeKey</span></span>|<span data-ttu-id="b249e-110">String</span><span class="sxs-lookup"><span data-stu-id="b249e-110">String</span></span>|<span data-ttu-id="b249e-p101">Указывает версию напоминания. При каждом изменении напоминания также меняется значение **changeKey**. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="b249e-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="b249e-114">Евентендтиме</span><span class="sxs-lookup"><span data-stu-id="b249e-114">eventEndTime</span></span>|[<span data-ttu-id="b249e-115">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b249e-115">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b249e-116">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="b249e-116">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="b249e-117">Диапазоне</span><span class="sxs-lookup"><span data-stu-id="b249e-117">eventId</span></span>|<span data-ttu-id="b249e-118">String</span><span class="sxs-lookup"><span data-stu-id="b249e-118">String</span></span>|<span data-ttu-id="b249e-p102">Уникальный идентификатор события. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b249e-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="b249e-121">Евентлокатион</span><span class="sxs-lookup"><span data-stu-id="b249e-121">eventLocation</span></span>|[<span data-ttu-id="b249e-122">Location</span><span class="sxs-lookup"><span data-stu-id="b249e-122">Location</span></span>](location.md)|<span data-ttu-id="b249e-123">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="b249e-123">The location of the event.</span></span>|
|<span data-ttu-id="b249e-124">Евентстарттиме</span><span class="sxs-lookup"><span data-stu-id="b249e-124">eventStartTime</span></span>|[<span data-ttu-id="b249e-125">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b249e-125">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b249e-126">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="b249e-126">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="b249e-127">Евентсубжект</span><span class="sxs-lookup"><span data-stu-id="b249e-127">eventSubject</span></span>|<span data-ttu-id="b249e-128">String</span><span class="sxs-lookup"><span data-stu-id="b249e-128">String</span></span>|<span data-ttu-id="b249e-129">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="b249e-129">The text of the event's subject line.</span></span>|
|<span data-ttu-id="b249e-130">Евентвеблинк</span><span class="sxs-lookup"><span data-stu-id="b249e-130">eventWebLink</span></span>|<span data-ttu-id="b249e-131">String</span><span class="sxs-lookup"><span data-stu-id="b249e-131">String</span></span>|<span data-ttu-id="b249e-132">URL-адрес для открытия события в Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="b249e-132">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="b249e-p103">Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.</span><span class="sxs-lookup"><span data-stu-id="b249e-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="b249e-135">Доступ к этому URL-адресу можно получить из объекта iFrame.</span><span class="sxs-lookup"><span data-stu-id="b249e-135">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="b249e-136">Реминдерфиретиме</span><span class="sxs-lookup"><span data-stu-id="b249e-136">reminderFireTime</span></span>|[<span data-ttu-id="b249e-137">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="b249e-137">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="b249e-138">Дата, время и часовой пояс, заданные для упоминания.</span><span class="sxs-lookup"><span data-stu-id="b249e-138">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b249e-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b249e-139">JSON representation</span></span>

<span data-ttu-id="b249e-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b249e-140">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "reminder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
