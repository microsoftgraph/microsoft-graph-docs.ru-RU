---
title: Тип ресурса toneInfo
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: b4ed9667c2e2156f52703c6fa15f4937ead5cef4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082107"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="57ec0-103">Тип ресурса toneInfo</span><span class="sxs-lookup"><span data-stu-id="57ec0-103">toneInfo resource type</span></span>

> <span data-ttu-id="57ec0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="57ec0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57ec0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="57ec0-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="57ec0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="57ec0-106">Properties</span></span>

| <span data-ttu-id="57ec0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="57ec0-107">Property</span></span>       | <span data-ttu-id="57ec0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="57ec0-108">Type</span></span>    | <span data-ttu-id="57ec0-109">Description</span><span class="sxs-lookup"><span data-stu-id="57ec0-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="57ec0-110">sequenceId</span><span class="sxs-lookup"><span data-stu-id="57ec0-110">sequenceId</span></span> | <span data-ttu-id="57ec0-111">Int64</span><span class="sxs-lookup"><span data-stu-id="57ec0-111">Int64</span></span> | <span data-ttu-id="57ec0-112">Добавочный идентификатор, используемый для сортировки событий DTMF.</span><span class="sxs-lookup"><span data-stu-id="57ec0-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="57ec0-113">сигнал</span><span class="sxs-lookup"><span data-stu-id="57ec0-113">tone</span></span> | <span data-ttu-id="57ec0-114">String</span><span class="sxs-lookup"><span data-stu-id="57ec0-114">String</span></span> | <span data-ttu-id="57ec0-115">Возможные значения: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="57ec0-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="57ec0-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="57ec0-116">JSON representation</span></span>

<span data-ttu-id="57ec0-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="57ec0-117">The following is a JSON representation of the resource.</span></span>

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