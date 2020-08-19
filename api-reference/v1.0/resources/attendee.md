---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 858018ac269fdf16929e2f0efea6ec40bada7639
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808363"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="ecb57-104">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="ecb57-104">attendee resource type</span></span>

<span data-ttu-id="ecb57-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecb57-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ecb57-106">Участник события.</span><span class="sxs-lookup"><span data-stu-id="ecb57-106">An event attendee.</span></span> <span data-ttu-id="ecb57-107">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="ecb57-107">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="ecb57-108">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="ecb57-108">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ecb57-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ecb57-109">Properties</span></span>
| <span data-ttu-id="ecb57-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecb57-110">Property</span></span>     | <span data-ttu-id="ecb57-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ecb57-111">Type</span></span>   |<span data-ttu-id="ecb57-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ecb57-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb57-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ecb57-113">emailAddress</span></span>|[<span data-ttu-id="ecb57-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ecb57-114">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="ecb57-115">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="ecb57-115">Includes the name and SMTP address of the attendee.</span></span>|
|<span data-ttu-id="ecb57-116">пропоседневтиме</span><span class="sxs-lookup"><span data-stu-id="ecb57-116">proposedNewTime</span></span>|[<span data-ttu-id="ecb57-117">timeSlot</span><span class="sxs-lookup"><span data-stu-id="ecb57-117">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="ecb57-118">Альтернативная дата/время, предлагаемая участником для начала и конца приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="ecb57-118">An alternate date/time proposed by the attendee for a meeting request to start and end.</span></span> <span data-ttu-id="ecb57-119">Если участник не предложил другое время, это свойство не включается в ответ на событие GET.</span><span class="sxs-lookup"><span data-stu-id="ecb57-119">If the attendee hasn't proposed another time, then this property is not included in a response of a GET event.</span></span>|
|<span data-ttu-id="ecb57-120">status</span><span class="sxs-lookup"><span data-stu-id="ecb57-120">status</span></span>|[<span data-ttu-id="ecb57-121">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="ecb57-121">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="ecb57-122">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="ecb57-122">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="ecb57-123">type</span><span class="sxs-lookup"><span data-stu-id="ecb57-123">type</span></span>|<span data-ttu-id="ecb57-124">String</span><span class="sxs-lookup"><span data-stu-id="ecb57-124">String</span></span>|<span data-ttu-id="ecb57-125">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="ecb57-125">The attendee type: `required`, `optional`, `resource`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ecb57-126">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ecb57-126">JSON representation</span></span>

<span data-ttu-id="ecb57-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecb57-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
  "optionalProperties": [
   "proposedNewTime"
  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
