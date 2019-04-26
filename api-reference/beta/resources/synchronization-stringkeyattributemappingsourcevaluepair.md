---
title: Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир
description: Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — Аттрибутемаппингсаурце.
localization_priority: Normal
ms.openlocfilehash: 7b722fb681ceb64ac4dd58553010e704e7669584
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345523"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="79845-103">Тип ресурса Стрингкэйаттрибутемаппингсаурцевалуепаир</span><span class="sxs-lookup"><span data-stu-id="79845-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79845-104">Представляет собой комбинацию "ключ-значение", в которой ключ является строкой, а значение — [аттрибутемаппингсаурце](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="79845-104">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="79845-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="79845-105">Properties</span></span>
| <span data-ttu-id="79845-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="79845-106">Property</span></span>     | <span data-ttu-id="79845-107">Тип</span><span class="sxs-lookup"><span data-stu-id="79845-107">Type</span></span>   |<span data-ttu-id="79845-108">Описание</span><span class="sxs-lookup"><span data-stu-id="79845-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79845-109">key</span><span class="sxs-lookup"><span data-stu-id="79845-109">key</span></span>|<span data-ttu-id="79845-110">String</span><span class="sxs-lookup"><span data-stu-id="79845-110">String</span></span>|<span data-ttu-id="79845-111">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="79845-111">The name of the parameter.</span></span>|
|<span data-ttu-id="79845-112">значение</span><span class="sxs-lookup"><span data-stu-id="79845-112">value</span></span>|[<span data-ttu-id="79845-113">Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="79845-113">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="79845-114">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="79845-114">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="79845-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="79845-115">JSON representation</span></span>

<span data-ttu-id="79845-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79845-116">The following is a JSON representation of the resource.</span></span>

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
