---
title: Тип ресурса stringKeyAttributeMappingSourceValuePair
description: Представляет пару "ключ-значение", где ключ является строкой, а значением является attributeMappingSource.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d0bd761b64c41c930bda84b820d98501870e0c26
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135100"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="e7d43-103">Тип ресурса stringKeyAttributeMappingSourceValuePair</span><span class="sxs-lookup"><span data-stu-id="e7d43-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

<span data-ttu-id="e7d43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7d43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7d43-105">Представляет пару "ключ-значение", где ключ является строкой, а [значением является attributeMappingSource.](synchronization-attributemappingsource.md)</span><span class="sxs-lookup"><span data-stu-id="e7d43-105">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e7d43-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e7d43-106">Properties</span></span>
| <span data-ttu-id="e7d43-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e7d43-107">Property</span></span>     | <span data-ttu-id="e7d43-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e7d43-108">Type</span></span>   |<span data-ttu-id="e7d43-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e7d43-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7d43-110">key</span><span class="sxs-lookup"><span data-stu-id="e7d43-110">key</span></span>|<span data-ttu-id="e7d43-111">Строка</span><span class="sxs-lookup"><span data-stu-id="e7d43-111">String</span></span>|<span data-ttu-id="e7d43-112">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="e7d43-112">The name of the parameter.</span></span>|
|<span data-ttu-id="e7d43-113">значение</span><span class="sxs-lookup"><span data-stu-id="e7d43-113">value</span></span>|[<span data-ttu-id="e7d43-114">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="e7d43-114">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="e7d43-115">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="e7d43-115">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7d43-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e7d43-116">JSON representation</span></span>

<span data-ttu-id="e7d43-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e7d43-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


