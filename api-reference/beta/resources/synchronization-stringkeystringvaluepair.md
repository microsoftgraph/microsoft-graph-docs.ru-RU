---
title: Тип ресурса stringKeyStringValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — это строка.
ms.openlocfilehash: 012625d78c8e07b3d38acba063acb57c751ced32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081862"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="7dc35-103">Тип ресурса stringKeyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="7dc35-103">stringKeyStringValuePair resource type</span></span>

> <span data-ttu-id="7dc35-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7dc35-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7dc35-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7dc35-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7dc35-106">Представляет пару ключ значение, где ключ — это строка, а значение — это строка.</span><span class="sxs-lookup"><span data-stu-id="7dc35-106">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="7dc35-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7dc35-107">Properties</span></span>
| <span data-ttu-id="7dc35-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7dc35-108">Property</span></span>     | <span data-ttu-id="7dc35-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7dc35-109">Type</span></span>   |<span data-ttu-id="7dc35-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7dc35-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7dc35-111">key</span><span class="sxs-lookup"><span data-stu-id="7dc35-111">key</span></span>|<span data-ttu-id="7dc35-112">String</span><span class="sxs-lookup"><span data-stu-id="7dc35-112">String</span></span>|<span data-ttu-id="7dc35-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="7dc35-113">Key.</span></span>|
|<span data-ttu-id="7dc35-114">value</span><span class="sxs-lookup"><span data-stu-id="7dc35-114">value</span></span>|<span data-ttu-id="7dc35-115">String</span><span class="sxs-lookup"><span data-stu-id="7dc35-115">String</span></span>|<span data-ttu-id="7dc35-116">Значение</span><span class="sxs-lookup"><span data-stu-id="7dc35-116">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7dc35-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7dc35-117">JSON representation</span></span>

<span data-ttu-id="7dc35-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7dc35-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->