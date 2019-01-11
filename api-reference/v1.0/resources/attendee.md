---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
ms.openlocfilehash: 89c289a342bb0b761bed982f88d0f47470eaa237
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856541"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="a082a-104">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="a082a-104">attendee resource type</span></span>

<span data-ttu-id="a082a-105">Участник события.</span><span class="sxs-lookup"><span data-stu-id="a082a-105">An event attendee.</span></span> <span data-ttu-id="a082a-106">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="a082a-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="a082a-107">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="a082a-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a082a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a082a-108">Properties</span></span>
| <span data-ttu-id="a082a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a082a-109">Property</span></span>     | <span data-ttu-id="a082a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a082a-110">Type</span></span>   |<span data-ttu-id="a082a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a082a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a082a-112">status</span><span class="sxs-lookup"><span data-stu-id="a082a-112">status</span></span>|[<span data-ttu-id="a082a-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="a082a-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="a082a-114">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="a082a-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="a082a-115">type</span><span class="sxs-lookup"><span data-stu-id="a082a-115">type</span></span>|<span data-ttu-id="a082a-116">String</span><span class="sxs-lookup"><span data-stu-id="a082a-116">String</span></span>|<span data-ttu-id="a082a-117">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="a082a-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="a082a-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a082a-118">emailAddress</span></span>|[<span data-ttu-id="a082a-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a082a-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a082a-120">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="a082a-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a082a-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a082a-121">JSON representation</span></span>

<span data-ttu-id="a082a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a082a-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attendeeBase",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
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
