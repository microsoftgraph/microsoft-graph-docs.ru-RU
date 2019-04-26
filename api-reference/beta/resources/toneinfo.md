---
title: Тип ресурса Тонеинфо
description: Одно событие DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9cf89df775bb663fbfb4c844b98c6cb35d085aa4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345493"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="b2e7a-103">Тип ресурса Тонеинфо</span><span class="sxs-lookup"><span data-stu-id="b2e7a-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2e7a-104">Одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="b2e7a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2e7a-105">Properties</span></span>

| <span data-ttu-id="b2e7a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2e7a-106">Property</span></span>       | <span data-ttu-id="b2e7a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b2e7a-107">Type</span></span>    | <span data-ttu-id="b2e7a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b2e7a-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b2e7a-109">Секуенцеид</span><span class="sxs-lookup"><span data-stu-id="b2e7a-109">sequenceId</span></span> | <span data-ttu-id="b2e7a-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b2e7a-110">Int64</span></span> | <span data-ttu-id="b2e7a-111">Добавочный идентификатор, используемый для упорядочивания событий DTMF.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="b2e7a-112">Новая</span><span class="sxs-lookup"><span data-stu-id="b2e7a-112">tone</span></span> | <span data-ttu-id="b2e7a-113">String</span><span class="sxs-lookup"><span data-stu-id="b2e7a-113">String</span></span> | <span data-ttu-id="b2e7a-114">Возможные значения: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`,. `flash`</span><span class="sxs-lookup"><span data-stu-id="b2e7a-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2e7a-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b2e7a-115">JSON representation</span></span>

<span data-ttu-id="b2e7a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2e7a-116">The following is a JSON representation of the resource.</span></span>

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
