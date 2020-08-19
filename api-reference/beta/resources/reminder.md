---
title: Тип ресурса reminder
description: Напоминание о событии в календаре пользователя.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: harini84
ms.openlocfilehash: 906e860cd6bab507a0acf89d561ccd8aeb1d1468
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812462"
---
# <a name="reminder-resource-type"></a><span data-ttu-id="9f6b1-103">Тип ресурса reminder</span><span class="sxs-lookup"><span data-stu-id="9f6b1-103">reminder resource type</span></span>

<span data-ttu-id="9f6b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f6b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f6b1-105">Напоминание о [событии](event.md) в [календаре](calendar.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-105">A reminder for an [event](event.md) in a user [calendar](calendar.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9f6b1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f6b1-106">Properties</span></span>
| <span data-ttu-id="9f6b1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f6b1-107">Property</span></span>     | <span data-ttu-id="9f6b1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9f6b1-108">Type</span></span>   |<span data-ttu-id="9f6b1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9f6b1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f6b1-110">changeKey</span><span class="sxs-lookup"><span data-stu-id="9f6b1-110">changeKey</span></span>|<span data-ttu-id="9f6b1-111">String</span><span class="sxs-lookup"><span data-stu-id="9f6b1-111">String</span></span>|<span data-ttu-id="9f6b1-p101">Указывает версию напоминания. При каждом изменении напоминания также меняется значение **changeKey**. Благодаря этому Exchange может применять изменения к правильной версии объекта.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-p101">Identifies the version of the reminder. Every time the reminder is changed, **changeKey** changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="9f6b1-115">евентендтиме</span><span class="sxs-lookup"><span data-stu-id="9f6b1-115">eventEndTime</span></span>|[<span data-ttu-id="9f6b1-116">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9f6b1-116">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9f6b1-117">Дата, время и часовой пояс завершения события.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-117">The date, time and time zone that the event ends.</span></span>|
|<span data-ttu-id="9f6b1-118">Диапазоне</span><span class="sxs-lookup"><span data-stu-id="9f6b1-118">eventId</span></span>|<span data-ttu-id="9f6b1-119">String</span><span class="sxs-lookup"><span data-stu-id="9f6b1-119">String</span></span>|<span data-ttu-id="9f6b1-p102">Уникальный идентификатор события. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-p102">The unique ID of the event. Read only.</span></span>|
|<span data-ttu-id="9f6b1-122">евентлокатион</span><span class="sxs-lookup"><span data-stu-id="9f6b1-122">eventLocation</span></span>|[<span data-ttu-id="9f6b1-123">Location</span><span class="sxs-lookup"><span data-stu-id="9f6b1-123">Location</span></span>](location.md)|<span data-ttu-id="9f6b1-124">Место проведения события.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-124">The location of the event.</span></span>|
|<span data-ttu-id="9f6b1-125">евентстарттиме</span><span class="sxs-lookup"><span data-stu-id="9f6b1-125">eventStartTime</span></span>|[<span data-ttu-id="9f6b1-126">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9f6b1-126">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9f6b1-127">Дата, время и часовой пояс начала события.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-127">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="9f6b1-128">евентсубжект</span><span class="sxs-lookup"><span data-stu-id="9f6b1-128">eventSubject</span></span>|<span data-ttu-id="9f6b1-129">String</span><span class="sxs-lookup"><span data-stu-id="9f6b1-129">String</span></span>|<span data-ttu-id="9f6b1-130">Текст в строке темы сообщения о событии.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-130">The text of the event's subject line.</span></span>|
|<span data-ttu-id="9f6b1-131">евентвеблинк</span><span class="sxs-lookup"><span data-stu-id="9f6b1-131">eventWebLink</span></span>|<span data-ttu-id="9f6b1-132">String</span><span class="sxs-lookup"><span data-stu-id="9f6b1-132">String</span></span>|<span data-ttu-id="9f6b1-133">URL-адрес для открытия события в Outlook в Интернете.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-133">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="9f6b1-p103">Событие откроется в браузере, если вы вошли в свой почтовый ящик с помощью Outlook в Интернете. Если вход с помощью браузера еще не выполнен, вам будет предложено войти.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-p103">The event will open in the browser if you are logged in to your mailbox via Outlook on the web. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="9f6b1-136">Доступ к этому URL-адресу можно получить из объекта iFrame.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-136">This URL can be accessed from within an iFrame.</span></span>|
|<span data-ttu-id="9f6b1-137">реминдерфиретиме</span><span class="sxs-lookup"><span data-stu-id="9f6b1-137">reminderFireTime</span></span>|[<span data-ttu-id="9f6b1-138">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="9f6b1-138">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="9f6b1-139">Дата, время и часовой пояс, заданные для упоминания.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-139">The date, time, and time zone that the reminder is set to occur.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f6b1-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9f6b1-140">JSON representation</span></span>

<span data-ttu-id="9f6b1-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f6b1-141">Here is a JSON representation of the resource</span></span>

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
