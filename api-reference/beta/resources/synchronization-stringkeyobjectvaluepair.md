---
title: Тип ресурса Стрингкэйобжектвалуепаир
description: Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON. Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9a04df77ee010368b73abfe5a2d8d78cfe99b0b4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217565"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="5b6d0-104">Тип ресурса Стрингкэйобжектвалуепаир</span><span class="sxs-lookup"><span data-stu-id="5b6d0-104">stringKeyObjectValuePair resource type</span></span>

<span data-ttu-id="5b6d0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b6d0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b6d0-106">Представляет собой запись "ключ-значение", в которой ключ является строкой, а значение — произвольным объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-106">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="5b6d0-107">Это открытый тип OData, который предполагает наличие свойства с именем `value` , которое является допустимым объектом JSON.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-107">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="5b6d0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b6d0-108">Properties</span></span>
| <span data-ttu-id="5b6d0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b6d0-109">Property</span></span>     | <span data-ttu-id="5b6d0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5b6d0-110">Type</span></span>   |<span data-ttu-id="5b6d0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5b6d0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b6d0-112">ключа</span><span class="sxs-lookup"><span data-stu-id="5b6d0-112">key</span></span>|<span data-ttu-id="5b6d0-113">Строка</span><span class="sxs-lookup"><span data-stu-id="5b6d0-113">String</span></span>|<span data-ttu-id="5b6d0-114">Ключ.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-114">Key.</span></span>|
|<span data-ttu-id="5b6d0-115">значение</span><span class="sxs-lookup"><span data-stu-id="5b6d0-115">value</span></span>|<span data-ttu-id="5b6d0-116">Json</span><span class="sxs-lookup"><span data-stu-id="5b6d0-116">Json</span></span>|<span data-ttu-id="5b6d0-117">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-117">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b6d0-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b6d0-118">JSON representation</span></span>

<span data-ttu-id="5b6d0-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b6d0-119">The following is a JSON representation of the resource.</span></span>

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
