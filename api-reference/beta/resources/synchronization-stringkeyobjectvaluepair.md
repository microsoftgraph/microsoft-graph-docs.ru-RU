---
title: Тип ресурса Стрингкэйобжектвалуепаир
description: Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c3a86cd4963f8d17fbe9f4c5371e98070f8f8f4e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520095"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="3b7e5-104">Тип ресурса Стрингкэйобжектвалуепаир</span><span class="sxs-lookup"><span data-stu-id="3b7e5-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="3b7e5-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b7e5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b7e5-106">Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="3b7e5-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="3b7e5-107">Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="3b7e5-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="3b7e5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3b7e5-108">Properties</span></span>
| <span data-ttu-id="3b7e5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3b7e5-109">Property</span></span>     | <span data-ttu-id="3b7e5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3b7e5-110">Type</span></span>   |<span data-ttu-id="3b7e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3b7e5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b7e5-112">ключа</span><span class="sxs-lookup"><span data-stu-id="3b7e5-112">key</span></span>|<span data-ttu-id="3b7e5-113">String</span><span class="sxs-lookup"><span data-stu-id="3b7e5-113">String</span></span>|<span data-ttu-id="3b7e5-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="3b7e5-114">Key.</span></span>|
|<span data-ttu-id="3b7e5-115">значение</span><span class="sxs-lookup"><span data-stu-id="3b7e5-115">value</span></span>|<span data-ttu-id="3b7e5-116">Json</span><span class="sxs-lookup"><span data-stu-id="3b7e5-116">Json</span></span>|<span data-ttu-id="3b7e5-117">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="3b7e5-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b7e5-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3b7e5-118">JSON representation</span></span>

<span data-ttu-id="3b7e5-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3b7e5-119">The following is a JSON representation of the resource.</span></span>

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
