---
title: Тип ресурса toneInfo
description: Одно событие DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b9be7e0e69be8d127df92f717ab462021f9684b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817110"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="5cf62-103">Тип ресурса toneInfo</span><span class="sxs-lookup"><span data-stu-id="5cf62-103">toneInfo resource type</span></span>

> <span data-ttu-id="5cf62-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5cf62-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cf62-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5cf62-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5cf62-106">Одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="5cf62-106">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="5cf62-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5cf62-107">Properties</span></span>

| <span data-ttu-id="5cf62-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5cf62-108">Property</span></span>       | <span data-ttu-id="5cf62-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5cf62-109">Type</span></span>    | <span data-ttu-id="5cf62-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5cf62-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5cf62-111">sequenceId</span><span class="sxs-lookup"><span data-stu-id="5cf62-111">sequenceId</span></span> | <span data-ttu-id="5cf62-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5cf62-112">Int64</span></span> | <span data-ttu-id="5cf62-113">Добавочный идентификатор, используемый для сортировки событий DTMF.</span><span class="sxs-lookup"><span data-stu-id="5cf62-113">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="5cf62-114">сигнал</span><span class="sxs-lookup"><span data-stu-id="5cf62-114">tone</span></span> | <span data-ttu-id="5cf62-115">Строка</span><span class="sxs-lookup"><span data-stu-id="5cf62-115">String</span></span> | <span data-ttu-id="5cf62-116">Возможные значения: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="5cf62-116">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5cf62-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5cf62-117">JSON representation</span></span>

<span data-ttu-id="5cf62-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5cf62-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
