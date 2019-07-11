---
title: Тип ресурса Стрингкэйобжектвалуепаир
description: Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b97f1f8bf10005a9e7829ee9280ebf936405b346
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620635"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="421fc-104">Тип ресурса Стрингкэйобжектвалуепаир</span><span class="sxs-lookup"><span data-stu-id="421fc-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="421fc-105">Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="421fc-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="421fc-106">Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="421fc-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="421fc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="421fc-107">Properties</span></span>
| <span data-ttu-id="421fc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="421fc-108">Property</span></span>     | <span data-ttu-id="421fc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="421fc-109">Type</span></span>   |<span data-ttu-id="421fc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="421fc-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="421fc-111">ключа</span><span class="sxs-lookup"><span data-stu-id="421fc-111">key</span></span>|<span data-ttu-id="421fc-112">String</span><span class="sxs-lookup"><span data-stu-id="421fc-112">String</span></span>|<span data-ttu-id="421fc-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="421fc-113">Key.</span></span>|
|<span data-ttu-id="421fc-114">значение</span><span class="sxs-lookup"><span data-stu-id="421fc-114">value</span></span>|<span data-ttu-id="421fc-115">Json</span><span class="sxs-lookup"><span data-stu-id="421fc-115">Json</span></span>|<span data-ttu-id="421fc-116">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="421fc-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="421fc-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="421fc-117">JSON representation</span></span>

<span data-ttu-id="421fc-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="421fc-118">The following is a JSON representation of the resource.</span></span>

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
