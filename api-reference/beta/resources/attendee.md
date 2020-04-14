---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: harini84
ms.openlocfilehash: f08734a9ec03c5e7e95a00abc5c95a9c968fa81c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472321"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="5156f-104">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="5156f-104">attendee resource type</span></span>

<span data-ttu-id="5156f-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5156f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5156f-106">Участник события.</span><span class="sxs-lookup"><span data-stu-id="5156f-106">An event attendee.</span></span> <span data-ttu-id="5156f-107">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="5156f-107">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="5156f-108">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="5156f-108">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5156f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="5156f-109">Properties</span></span>
| <span data-ttu-id="5156f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="5156f-110">Property</span></span>     | <span data-ttu-id="5156f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="5156f-111">Type</span></span>   |<span data-ttu-id="5156f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5156f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5156f-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5156f-113">emailAddress</span></span>|[<span data-ttu-id="5156f-114">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5156f-114">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="5156f-115">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="5156f-115">Includes the name and SMTP address of the attendee.</span></span>|
|<span data-ttu-id="5156f-116">пропоседневтиме</span><span class="sxs-lookup"><span data-stu-id="5156f-116">proposedNewTime</span></span>|[<span data-ttu-id="5156f-117">timeSlot</span><span class="sxs-lookup"><span data-stu-id="5156f-117">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="5156f-118">Альтернативная дата/время, предлагаемая участником для начала и конца приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="5156f-118">An alternate date/time proposed by the attendee for a meeting request to start and end.</span></span> <span data-ttu-id="5156f-119">Если участник не предложил другое время, это свойство не включается в ответ на событие GET.</span><span class="sxs-lookup"><span data-stu-id="5156f-119">If the attendee hasn't proposed another time, then this property is not included in a response of a GET event.</span></span>|
|<span data-ttu-id="5156f-120">status</span><span class="sxs-lookup"><span data-stu-id="5156f-120">status</span></span>|[<span data-ttu-id="5156f-121">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="5156f-121">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="5156f-122">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="5156f-122">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="5156f-123">type</span><span class="sxs-lookup"><span data-stu-id="5156f-123">type</span></span>|<span data-ttu-id="5156f-124">String</span><span class="sxs-lookup"><span data-stu-id="5156f-124">String</span></span>|<span data-ttu-id="5156f-125">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="5156f-125">The attendee type: `required`, `optional`, `resource`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5156f-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5156f-126">JSON representation</span></span>

<span data-ttu-id="5156f-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5156f-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
