---
title: Тип ресурса patternedRecurrence
description: Расписание и диапазон повторения.
ms.openlocfilehash: 205c563d8b4cecc0a817dd1893a6c4f002eb4e06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082657"
---
# <a name="patternedrecurrence-resource-type"></a><span data-ttu-id="faf34-103">Тип ресурса patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="faf34-103">patternedRecurrence resource type</span></span>

> <span data-ttu-id="faf34-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="faf34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="faf34-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="faf34-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="faf34-106">Расписание и диапазон повторения.</span><span class="sxs-lookup"><span data-stu-id="faf34-106">The recurrence pattern and range.</span></span>

## <a name="properties"></a><span data-ttu-id="faf34-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="faf34-107">Properties</span></span>
| <span data-ttu-id="faf34-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="faf34-108">Property</span></span>     | <span data-ttu-id="faf34-109">Тип</span><span class="sxs-lookup"><span data-stu-id="faf34-109">Type</span></span>   |<span data-ttu-id="faf34-110">Описание</span><span class="sxs-lookup"><span data-stu-id="faf34-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faf34-111">pattern</span><span class="sxs-lookup"><span data-stu-id="faf34-111">pattern</span></span>|[<span data-ttu-id="faf34-112">RecurrencePattern</span><span class="sxs-lookup"><span data-stu-id="faf34-112">RecurrencePattern</span></span>](recurrencepattern.md)|<span data-ttu-id="faf34-113">Частота события.</span><span class="sxs-lookup"><span data-stu-id="faf34-113">The frequency of an event.</span></span>|
|<span data-ttu-id="faf34-114">range</span><span class="sxs-lookup"><span data-stu-id="faf34-114">range</span></span>|[<span data-ttu-id="faf34-115">RecurrenceRange</span><span class="sxs-lookup"><span data-stu-id="faf34-115">RecurrenceRange</span></span>](recurrencerange.md)|<span data-ttu-id="faf34-116">Продолжительность события.</span><span class="sxs-lookup"><span data-stu-id="faf34-116">The duration of an event.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="faf34-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="faf34-117">JSON representation</span></span>

<span data-ttu-id="faf34-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="faf34-118">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
