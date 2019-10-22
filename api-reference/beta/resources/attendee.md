---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: 4e906a2f7f9d95cd3c3623d1f84c41aedded6cc4
ms.sourcegitcommit: c9b9ff2c862f8d96d282a7bdf641cdb9c53a4600
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2019
ms.locfileid: "37621589"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="455da-104">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="455da-104">attendee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="455da-105">Участник события.</span><span class="sxs-lookup"><span data-stu-id="455da-105">An event attendee.</span></span> <span data-ttu-id="455da-106">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="455da-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="455da-107">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="455da-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="455da-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="455da-108">Properties</span></span>
| <span data-ttu-id="455da-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="455da-109">Property</span></span>     | <span data-ttu-id="455da-110">Тип</span><span class="sxs-lookup"><span data-stu-id="455da-110">Type</span></span>   |<span data-ttu-id="455da-111">Описание</span><span class="sxs-lookup"><span data-stu-id="455da-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="455da-112">emailAddress</span><span class="sxs-lookup"><span data-stu-id="455da-112">emailAddress</span></span>|[<span data-ttu-id="455da-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="455da-113">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="455da-114">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="455da-114">Includes the name and SMTP address of the attendee.</span></span>|
|<span data-ttu-id="455da-115">пропоседневтиме</span><span class="sxs-lookup"><span data-stu-id="455da-115">proposedNewTime</span></span>|[<span data-ttu-id="455da-116">timeSlot</span><span class="sxs-lookup"><span data-stu-id="455da-116">timeSlot</span></span>](timeslot.md)|<span data-ttu-id="455da-117">Альтернативная дата/время, предлагаемая участником для начала и конца приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="455da-117">An alternate date/time proposed by the attendee for a meeting request to start and end.</span></span> <span data-ttu-id="455da-118">Если участник не предложил другое время, это свойство не включается в ответ на событие GET.</span><span class="sxs-lookup"><span data-stu-id="455da-118">If the attendee hasn't proposed another time, then this property is not included in a response of a GET event.</span></span>|
|<span data-ttu-id="455da-119">status</span><span class="sxs-lookup"><span data-stu-id="455da-119">status</span></span>|[<span data-ttu-id="455da-120">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="455da-120">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="455da-121">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="455da-121">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="455da-122">type</span><span class="sxs-lookup"><span data-stu-id="455da-122">type</span></span>|<span data-ttu-id="455da-123">String</span><span class="sxs-lookup"><span data-stu-id="455da-123">String</span></span>|<span data-ttu-id="455da-124">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="455da-124">The attendee type: `required`, `optional`, `resource`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="455da-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="455da-125">JSON representation</span></span>

<span data-ttu-id="455da-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="455da-126">Here is a JSON representation of the resource</span></span>

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
