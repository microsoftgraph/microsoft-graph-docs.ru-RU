---
title: Тип ресурса stringKeyObjectValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON. Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.
ms.openlocfilehash: ae536b2aab87b9920c2afcbe324e30b5f5380dbb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078352"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="1504e-104">Тип ресурса stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="1504e-104">stringKeyObjectValuePair resource type</span></span>

> <span data-ttu-id="1504e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1504e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1504e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1504e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1504e-107">Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="1504e-107">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="1504e-108">Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.</span><span class="sxs-lookup"><span data-stu-id="1504e-108">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="1504e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1504e-109">Properties</span></span>
| <span data-ttu-id="1504e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1504e-110">Property</span></span>     | <span data-ttu-id="1504e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1504e-111">Type</span></span>   |<span data-ttu-id="1504e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1504e-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1504e-113">key</span><span class="sxs-lookup"><span data-stu-id="1504e-113">key</span></span>|<span data-ttu-id="1504e-114">String</span><span class="sxs-lookup"><span data-stu-id="1504e-114">String</span></span>|<span data-ttu-id="1504e-115">Ключ.</span><span class="sxs-lookup"><span data-stu-id="1504e-115">Key.</span></span>|
|<span data-ttu-id="1504e-116">value</span><span class="sxs-lookup"><span data-stu-id="1504e-116">value</span></span>|<span data-ttu-id="1504e-117">Любой</span><span class="sxs-lookup"><span data-stu-id="1504e-117">Any</span></span>|<span data-ttu-id="1504e-118">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="1504e-118">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1504e-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1504e-119">JSON representation</span></span>

<span data-ttu-id="1504e-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1504e-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->