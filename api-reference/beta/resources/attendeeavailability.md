---
title: Тип ресурсов attendeeAvailability
description: Доступность участника.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 95896808f1a58eb77cafb8003ca5c7848d50bc08
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339031"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="fe24f-103">Тип ресурсов attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="fe24f-103">attendeeAvailability resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe24f-104">Доступность участника.</span><span class="sxs-lookup"><span data-stu-id="fe24f-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe24f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe24f-105">JSON representation</span></span>

<span data-ttu-id="fe24f-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="fe24f-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="fe24f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe24f-107">Properties</span></span>
| <span data-ttu-id="fe24f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe24f-108">Property</span></span>     | <span data-ttu-id="fe24f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fe24f-109">Type</span></span>   |<span data-ttu-id="fe24f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe24f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe24f-111">attendee</span><span class="sxs-lookup"><span data-stu-id="fe24f-111">attendee</span></span>|[<span data-ttu-id="fe24f-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="fe24f-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="fe24f-113">Адрес электронной почты и тип участника — является ли это пользователь или ресурс, а также является ли он обязательным, если это человек.</span><span class="sxs-lookup"><span data-stu-id="fe24f-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="fe24f-114">availability</span><span class="sxs-lookup"><span data-stu-id="fe24f-114">availability</span></span>|<span data-ttu-id="fe24f-115">Фрибусистатус</span><span class="sxs-lookup"><span data-stu-id="fe24f-115">freeBusyStatus</span></span>| <span data-ttu-id="fe24f-p101">Состояние занятости участника. Возможные значения: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fe24f-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
