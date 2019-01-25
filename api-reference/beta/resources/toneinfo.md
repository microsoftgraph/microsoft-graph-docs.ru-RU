---
title: Тип ресурса toneInfo
description: Одно событие DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f58548f8f075494c6601db2962d88fb6cabb59ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526013"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="380fd-103">Тип ресурса toneInfo</span><span class="sxs-lookup"><span data-stu-id="380fd-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="380fd-104">Одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="380fd-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="380fd-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="380fd-105">Properties</span></span>

| <span data-ttu-id="380fd-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="380fd-106">Property</span></span>       | <span data-ttu-id="380fd-107">Тип</span><span class="sxs-lookup"><span data-stu-id="380fd-107">Type</span></span>    | <span data-ttu-id="380fd-108">Описание</span><span class="sxs-lookup"><span data-stu-id="380fd-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="380fd-109">sequenceId</span><span class="sxs-lookup"><span data-stu-id="380fd-109">sequenceId</span></span> | <span data-ttu-id="380fd-110">Int64</span><span class="sxs-lookup"><span data-stu-id="380fd-110">Int64</span></span> | <span data-ttu-id="380fd-111">Добавочный идентификатор, используемый для сортировки событий DTMF.</span><span class="sxs-lookup"><span data-stu-id="380fd-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="380fd-112">сигнал</span><span class="sxs-lookup"><span data-stu-id="380fd-112">tone</span></span> | <span data-ttu-id="380fd-113">String</span><span class="sxs-lookup"><span data-stu-id="380fd-113">String</span></span> | <span data-ttu-id="380fd-114">Возможные значения: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="380fd-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="380fd-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="380fd-115">JSON representation</span></span>

<span data-ttu-id="380fd-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="380fd-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/toneinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
