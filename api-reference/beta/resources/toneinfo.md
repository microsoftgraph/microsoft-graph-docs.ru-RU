---
title: Тип ресурса Тонеинфо
description: Одно событие DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: aa0ef52126895e61300c1e2f7a258926e209866c
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006524"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="2f4fb-103">Тип ресурса Тонеинфо</span><span class="sxs-lookup"><span data-stu-id="2f4fb-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f4fb-104">Одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="2f4fb-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="2f4fb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f4fb-105">Properties</span></span>

| <span data-ttu-id="2f4fb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f4fb-106">Property</span></span>       | <span data-ttu-id="2f4fb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2f4fb-107">Type</span></span>    | <span data-ttu-id="2f4fb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2f4fb-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2f4fb-109">секуенцеид</span><span class="sxs-lookup"><span data-stu-id="2f4fb-109">sequenceId</span></span> | <span data-ttu-id="2f4fb-110">Int64</span><span class="sxs-lookup"><span data-stu-id="2f4fb-110">Int64</span></span> | <span data-ttu-id="2f4fb-111">Добавочный идентификатор, используемый для упорядочивания событий DTMF.</span><span class="sxs-lookup"><span data-stu-id="2f4fb-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="2f4fb-112">Новая</span><span class="sxs-lookup"><span data-stu-id="2f4fb-112">tone</span></span> | <span data-ttu-id="2f4fb-113">String</span><span class="sxs-lookup"><span data-stu-id="2f4fb-113">String</span></span> | <span data-ttu-id="2f4fb-114">Возможные значения: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`,. `flash`</span><span class="sxs-lookup"><span data-stu-id="2f4fb-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f4fb-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f4fb-115">JSON representation</span></span>

<span data-ttu-id="2f4fb-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f4fb-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
