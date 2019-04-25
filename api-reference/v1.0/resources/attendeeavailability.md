---
title: Тип ресурсов attendeeAvailability
description: Доступность участника.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63014553824b833e2e4cdfb03485fcb7962c01a0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569363"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="346e2-103">Тип ресурсов attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="346e2-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="346e2-104">Доступность участника.</span><span class="sxs-lookup"><span data-stu-id="346e2-104">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="346e2-105">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="346e2-105">JSON representation</span></span>

<span data-ttu-id="346e2-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="346e2-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="346e2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="346e2-107">Properties</span></span>
| <span data-ttu-id="346e2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="346e2-108">Property</span></span>     | <span data-ttu-id="346e2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="346e2-109">Type</span></span>   |<span data-ttu-id="346e2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="346e2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="346e2-111">attendee</span><span class="sxs-lookup"><span data-stu-id="346e2-111">attendee</span></span>|[<span data-ttu-id="346e2-112">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="346e2-112">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="346e2-113">Адрес электронной почты и тип участника — является ли это пользователь или ресурс, а также является ли он обязательным, если это человек.</span><span class="sxs-lookup"><span data-stu-id="346e2-113">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="346e2-114">availability</span><span class="sxs-lookup"><span data-stu-id="346e2-114">availability</span></span>|<span data-ttu-id="346e2-115">Фрибусистатус</span><span class="sxs-lookup"><span data-stu-id="346e2-115">freeBusyStatus</span></span>| <span data-ttu-id="346e2-116">Состояние занятости участника.</span><span class="sxs-lookup"><span data-stu-id="346e2-116">The availability status of the attendee.</span></span> <span data-ttu-id="346e2-117">Возможные `free`значения:, `tentative`, `busy`, `oof`, `workingElsewhere`,. `unknown`</span><span class="sxs-lookup"><span data-stu-id="346e2-117">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
