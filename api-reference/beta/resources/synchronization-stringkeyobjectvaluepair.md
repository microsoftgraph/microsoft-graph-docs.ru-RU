---
title: Тип ресурса stringKeyObjectValuePair
description: Представляет пару "ключ-значение", где ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который должен иметь свойство с именем, которое `value` является допустимым объектом JSON.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 535e9f104f42771e6f6c182769f0a5e1f68169b6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137069"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="f7323-104">Тип ресурса stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="f7323-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="f7323-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7323-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7323-106">Представляет пару "ключ-значение", где ключ является строкой, а значение — произвольным объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="f7323-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="f7323-107">Это открытый тип OData, который должен иметь свойство с именем, которое `value` является допустимым объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="f7323-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="f7323-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7323-108">Properties</span></span>
| <span data-ttu-id="f7323-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7323-109">Property</span></span>     | <span data-ttu-id="f7323-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f7323-110">Type</span></span>   |<span data-ttu-id="f7323-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f7323-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7323-112">key</span><span class="sxs-lookup"><span data-stu-id="f7323-112">key</span></span>|<span data-ttu-id="f7323-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f7323-113">String</span></span>|<span data-ttu-id="f7323-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="f7323-114">Key.</span></span>|
|<span data-ttu-id="f7323-115">значение</span><span class="sxs-lookup"><span data-stu-id="f7323-115">value</span></span>|<span data-ttu-id="f7323-116">Json</span><span class="sxs-lookup"><span data-stu-id="f7323-116">Json</span></span>|<span data-ttu-id="f7323-117">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="f7323-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7323-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f7323-118">JSON representation</span></span>

<span data-ttu-id="f7323-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7323-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


