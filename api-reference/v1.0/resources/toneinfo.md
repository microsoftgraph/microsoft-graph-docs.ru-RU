---
title: Тип ресурса Тонеинфо
description: Одно событие DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bd386d77dcd3122e1bcd243230062f47b17b5749
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090650"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="33869-103">Тип ресурса Тонеинфо</span><span class="sxs-lookup"><span data-stu-id="33869-103">toneInfo resource type</span></span>

<span data-ttu-id="33869-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33869-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33869-105">Одно событие DTMF.</span><span class="sxs-lookup"><span data-stu-id="33869-105">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="33869-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="33869-106">Properties</span></span>

| <span data-ttu-id="33869-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="33869-107">Property</span></span>       | <span data-ttu-id="33869-108">Тип</span><span class="sxs-lookup"><span data-stu-id="33869-108">Type</span></span>    | <span data-ttu-id="33869-109">Описание</span><span class="sxs-lookup"><span data-stu-id="33869-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="33869-110">секуенцеид</span><span class="sxs-lookup"><span data-stu-id="33869-110">sequenceId</span></span> | <span data-ttu-id="33869-111">Int64</span><span class="sxs-lookup"><span data-stu-id="33869-111">Int64</span></span> | <span data-ttu-id="33869-112">Добавочный идентификатор, используемый для упорядочивания событий DTMF.</span><span class="sxs-lookup"><span data-stu-id="33869-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="33869-113">Новая</span><span class="sxs-lookup"><span data-stu-id="33869-113">tone</span></span> | <span data-ttu-id="33869-114">Строка</span><span class="sxs-lookup"><span data-stu-id="33869-114">String</span></span> | <span data-ttu-id="33869-115">Возможные значения: `tone0` , `tone1` ,,,,, `tone2` `tone3` `tone4` `tone5` `tone6` ,,, `tone7` `tone8` `tone9` , `star` , `pound`</span><span class="sxs-lookup"><span data-stu-id="33869-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="33869-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33869-116">JSON representation</span></span>

<span data-ttu-id="33869-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33869-117">The following is a JSON representation of the resource.</span></span>

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

