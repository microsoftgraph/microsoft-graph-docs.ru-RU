---
title: Тип ресурса stringKeyObjectValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON. Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.
localization_priority: Normal
ms.openlocfilehash: 8545a4ef5a4931d3b886c95b4f39218bc418f53d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831453"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a><span data-ttu-id="4b092-104">Тип ресурса stringKeyObjectValuePair</span><span class="sxs-lookup"><span data-stu-id="4b092-104">stringKeyObjectValuePair resource type</span></span>

> <span data-ttu-id="4b092-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4b092-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b092-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4b092-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4b092-107">Представляет пару ключ значение, где ключ — это строка, а значение — это произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="4b092-107">Represents a key-value pair where the key is a string and the value is an arbitrary JSON object.</span></span> <span data-ttu-id="4b092-108">Это открытого типа OData, который будет использовать свойство с именем `value` то есть допустимый объект JSON.</span><span class="sxs-lookup"><span data-stu-id="4b092-108">This is an OData open type that expects to have a property named `value` that is a valid JSON object.</span></span>

## <a name="properties"></a><span data-ttu-id="4b092-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4b092-109">Properties</span></span>
| <span data-ttu-id="4b092-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4b092-110">Property</span></span>     | <span data-ttu-id="4b092-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4b092-111">Type</span></span>   |<span data-ttu-id="4b092-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4b092-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b092-113">key</span><span class="sxs-lookup"><span data-stu-id="4b092-113">key</span></span>|<span data-ttu-id="4b092-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4b092-114">String</span></span>|<span data-ttu-id="4b092-115">Ключ.</span><span class="sxs-lookup"><span data-stu-id="4b092-115">Key.</span></span>|
|<span data-ttu-id="4b092-116">value</span><span class="sxs-lookup"><span data-stu-id="4b092-116">value</span></span>|<span data-ttu-id="4b092-117">Любой</span><span class="sxs-lookup"><span data-stu-id="4b092-117">Any</span></span>|<span data-ttu-id="4b092-118">Произвольный объект JSON.</span><span class="sxs-lookup"><span data-stu-id="4b092-118">Arbitrary JSON object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b092-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4b092-119">JSON representation</span></span>

<span data-ttu-id="4b092-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4b092-120">The following is a JSON representation of the resource.</span></span>

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
