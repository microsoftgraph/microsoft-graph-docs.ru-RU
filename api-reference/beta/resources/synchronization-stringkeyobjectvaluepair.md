---
title: Тип ресурса Стрингкэйобжектвалуепаир
description: Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.
localization_priority: Normal
ms.openlocfilehash: 66b4438b73f0000c172db1df385088528d221be4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324804"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="71f79-104">Тип ресурса Стрингкэйобжектвалуепаир</span><span class="sxs-lookup"><span data-stu-id="71f79-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71f79-105">Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="71f79-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="71f79-106">Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="71f79-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="71f79-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="71f79-107">Properties</span></span>
| <span data-ttu-id="71f79-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="71f79-108">Property</span></span>     | <span data-ttu-id="71f79-109">Тип</span><span class="sxs-lookup"><span data-stu-id="71f79-109">Type</span></span>   |<span data-ttu-id="71f79-110">Описание</span><span class="sxs-lookup"><span data-stu-id="71f79-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="71f79-111">ключа</span><span class="sxs-lookup"><span data-stu-id="71f79-111">key</span></span>|<span data-ttu-id="71f79-112">String</span><span class="sxs-lookup"><span data-stu-id="71f79-112">String</span></span>|<span data-ttu-id="71f79-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="71f79-113">Key.</span></span>|
|<span data-ttu-id="71f79-114">значение</span><span class="sxs-lookup"><span data-stu-id="71f79-114">value</span></span>|<span data-ttu-id="71f79-115">Json</span><span class="sxs-lookup"><span data-stu-id="71f79-115">Json</span></span>|<span data-ttu-id="71f79-116">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="71f79-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="71f79-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="71f79-117">JSON representation</span></span>

<span data-ttu-id="71f79-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71f79-118">The following is a JSON representation of the resource.</span></span>

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
