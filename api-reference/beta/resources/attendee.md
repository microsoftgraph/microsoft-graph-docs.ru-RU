---
title: Тип ресурса attendee
description: Участник события. Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.
localization_priority: Normal
ms.openlocfilehash: d50b6756c7d0077ec95f10988d06fa2ff81631fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642879"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="a20e6-104">Тип ресурса attendee</span><span class="sxs-lookup"><span data-stu-id="a20e6-104">attendee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a20e6-105">Участник события.</span><span class="sxs-lookup"><span data-stu-id="a20e6-105">An event attendee.</span></span> <span data-ttu-id="a20e6-106">Это может быть человек или ресурс (например конференц-зал или оборудование), настроенный в качестве ресурса на сервере Exchange Server клиента.</span><span class="sxs-lookup"><span data-stu-id="a20e6-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="a20e6-107">Тип, производный от [attendeeBase](attendeebase.md).</span><span class="sxs-lookup"><span data-stu-id="a20e6-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a20e6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a20e6-108">Properties</span></span>
| <span data-ttu-id="a20e6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a20e6-109">Property</span></span>     | <span data-ttu-id="a20e6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a20e6-110">Type</span></span>   |<span data-ttu-id="a20e6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a20e6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a20e6-112">status</span><span class="sxs-lookup"><span data-stu-id="a20e6-112">status</span></span>|[<span data-ttu-id="a20e6-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="a20e6-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="a20e6-114">Ответ участника (нет, принято, отклонено и т. д.) на событие, а также дата и время отправки ответа.</span><span class="sxs-lookup"><span data-stu-id="a20e6-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="a20e6-115">type</span><span class="sxs-lookup"><span data-stu-id="a20e6-115">type</span></span>|<span data-ttu-id="a20e6-116">String</span><span class="sxs-lookup"><span data-stu-id="a20e6-116">String</span></span>|<span data-ttu-id="a20e6-117">Тип участника: `required`, `optional`, `resource`.</span><span class="sxs-lookup"><span data-stu-id="a20e6-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="a20e6-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a20e6-118">emailAddress</span></span>|[<span data-ttu-id="a20e6-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a20e6-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a20e6-120">Включает имя и SMTP-адрес участника.</span><span class="sxs-lookup"><span data-stu-id="a20e6-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a20e6-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a20e6-121">JSON representation</span></span>

<span data-ttu-id="a20e6-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a20e6-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/attendee.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
