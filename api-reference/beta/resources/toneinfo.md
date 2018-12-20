---
title: Тип ресурса toneInfo
description: Одно событие DTMF.
author: VinodRavichandran
ms.openlocfilehash: 0ae78a9a4721c88767ebc460a99c7cdea30f44c5
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380340"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="5bf13-103">Тип ресурса toneInfo</span><span class="sxs-lookup"><span data-stu-id="5bf13-103">toneInfo resource type</span></span>

> <span data-ttu-id="5bf13-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5bf13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5bf13-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5bf13-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5bf13-106">Одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="5bf13-106">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="5bf13-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5bf13-107">Properties</span></span>

| <span data-ttu-id="5bf13-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5bf13-108">Property</span></span>       | <span data-ttu-id="5bf13-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5bf13-109">Type</span></span>    | <span data-ttu-id="5bf13-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5bf13-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5bf13-111">sequenceId</span><span class="sxs-lookup"><span data-stu-id="5bf13-111">sequenceId</span></span> | <span data-ttu-id="5bf13-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5bf13-112">Int64</span></span> | <span data-ttu-id="5bf13-113">Добавочный идентификатор, используемый для сортировки событий DTMF.</span><span class="sxs-lookup"><span data-stu-id="5bf13-113">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="5bf13-114">сигнал</span><span class="sxs-lookup"><span data-stu-id="5bf13-114">tone</span></span> | <span data-ttu-id="5bf13-115">String</span><span class="sxs-lookup"><span data-stu-id="5bf13-115">String</span></span> | <span data-ttu-id="5bf13-116">Возможные значения: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="5bf13-116">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5bf13-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5bf13-117">JSON representation</span></span>

<span data-ttu-id="5bf13-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5bf13-118">The following is a JSON representation of the resource.</span></span>

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