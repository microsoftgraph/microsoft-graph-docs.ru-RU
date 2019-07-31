---
title: Тип ресурса Стрингкэйобжектвалуепаир
description: Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3ec55eee1f6b5f60e8936f906390d5343fbafbdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007832"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="c45cd-104">Тип ресурса Стрингкэйобжектвалуепаир</span><span class="sxs-lookup"><span data-stu-id="c45cd-104">stringKeyObjectValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c45cd-105">Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="c45cd-105">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="c45cd-106">Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="c45cd-106">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="c45cd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c45cd-107">Properties</span></span>
| <span data-ttu-id="c45cd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c45cd-108">Property</span></span>     | <span data-ttu-id="c45cd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c45cd-109">Type</span></span>   |<span data-ttu-id="c45cd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c45cd-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c45cd-111">ключа</span><span class="sxs-lookup"><span data-stu-id="c45cd-111">key</span></span>|<span data-ttu-id="c45cd-112">String</span><span class="sxs-lookup"><span data-stu-id="c45cd-112">String</span></span>|<span data-ttu-id="c45cd-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="c45cd-113">Key.</span></span>|
|<span data-ttu-id="c45cd-114">значение</span><span class="sxs-lookup"><span data-stu-id="c45cd-114">value</span></span>|<span data-ttu-id="c45cd-115">Json</span><span class="sxs-lookup"><span data-stu-id="c45cd-115">Json</span></span>|<span data-ttu-id="c45cd-116">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="c45cd-116">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c45cd-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c45cd-117">JSON representation</span></span>

<span data-ttu-id="c45cd-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c45cd-118">The following is a JSON representation of the resource.</span></span>

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
