---
title: Тип ресурса stringKeyAttributeMappingSourceValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — attributeMappingSource.
ms.openlocfilehash: 875c593ae652ce763f420d29e5dd4e5e2601bc88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081863"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="45697-103">Тип ресурса stringKeyAttributeMappingSourceValuePair</span><span class="sxs-lookup"><span data-stu-id="45697-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

> <span data-ttu-id="45697-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="45697-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45697-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45697-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45697-106">Представляет пару ключ значение, где ключ — это строка, а значение — [attributeMappingSource](synchronization-attributemappingsource.md).</span><span class="sxs-lookup"><span data-stu-id="45697-106">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="45697-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="45697-107">Properties</span></span>
| <span data-ttu-id="45697-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="45697-108">Property</span></span>     | <span data-ttu-id="45697-109">Тип</span><span class="sxs-lookup"><span data-stu-id="45697-109">Type</span></span>   |<span data-ttu-id="45697-110">Описание</span><span class="sxs-lookup"><span data-stu-id="45697-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45697-111">key</span><span class="sxs-lookup"><span data-stu-id="45697-111">key</span></span>|<span data-ttu-id="45697-112">String</span><span class="sxs-lookup"><span data-stu-id="45697-112">String</span></span>|<span data-ttu-id="45697-113">Имя параметра.</span><span class="sxs-lookup"><span data-stu-id="45697-113">The name of the parameter.</span></span>|
|<span data-ttu-id="45697-114">value</span><span class="sxs-lookup"><span data-stu-id="45697-114">value</span></span>|[<span data-ttu-id="45697-115">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="45697-115">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="45697-116">Значение параметра.</span><span class="sxs-lookup"><span data-stu-id="45697-116">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="45697-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="45697-117">JSON representation</span></span>

<span data-ttu-id="45697-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45697-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
