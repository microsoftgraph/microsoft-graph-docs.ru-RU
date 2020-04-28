---
title: Тип ресурса Тонеинфо
description: Одно событие DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 99889abd2d3d9272f4f0ecb9b4d1b5321029beea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519661"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="4bb12-103">Тип ресурса Тонеинфо</span><span class="sxs-lookup"><span data-stu-id="4bb12-103">toneInfo resource type</span></span>

<span data-ttu-id="4bb12-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bb12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bb12-105">Одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="4bb12-105">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="4bb12-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4bb12-106">Properties</span></span>

| <span data-ttu-id="4bb12-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4bb12-107">Property</span></span>       | <span data-ttu-id="4bb12-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4bb12-108">Type</span></span>    | <span data-ttu-id="4bb12-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4bb12-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4bb12-110">секуенцеид</span><span class="sxs-lookup"><span data-stu-id="4bb12-110">sequenceId</span></span> | <span data-ttu-id="4bb12-111">Int64</span><span class="sxs-lookup"><span data-stu-id="4bb12-111">Int64</span></span> | <span data-ttu-id="4bb12-112">Добавочный идентификатор, используемый для упорядочивания событий DTMF.</span><span class="sxs-lookup"><span data-stu-id="4bb12-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="4bb12-113">Новая</span><span class="sxs-lookup"><span data-stu-id="4bb12-113">tone</span></span> | <span data-ttu-id="4bb12-114">String</span><span class="sxs-lookup"><span data-stu-id="4bb12-114">String</span></span> | <span data-ttu-id="4bb12-115">Возможные значения: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`,. `flash`</span><span class="sxs-lookup"><span data-stu-id="4bb12-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4bb12-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4bb12-116">JSON representation</span></span>

<span data-ttu-id="4bb12-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4bb12-117">The following is a JSON representation of the resource.</span></span>

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
