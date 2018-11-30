---
title: Тип ресурса stringKeyLongValuePair
description: Представляет пару ключ значение, где ключ — это строка, а значение — Int64.
ms.openlocfilehash: 0ceafbc4ab683469e616e068c0abc00804578908
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081422"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="2171a-103">Тип ресурса stringKeyLongValuePair</span><span class="sxs-lookup"><span data-stu-id="2171a-103">stringKeyLongValuePair resource type</span></span>

> <span data-ttu-id="2171a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2171a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2171a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2171a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2171a-106">Представляет пару ключ значение, где ключ — это строка, а значение — Int64.</span><span class="sxs-lookup"><span data-stu-id="2171a-106">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="2171a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2171a-107">Properties</span></span>
| <span data-ttu-id="2171a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2171a-108">Property</span></span>     | <span data-ttu-id="2171a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2171a-109">Type</span></span>   |<span data-ttu-id="2171a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2171a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2171a-111">key</span><span class="sxs-lookup"><span data-stu-id="2171a-111">key</span></span>|<span data-ttu-id="2171a-112">String</span><span class="sxs-lookup"><span data-stu-id="2171a-112">String</span></span>|<span data-ttu-id="2171a-113">Ключ.</span><span class="sxs-lookup"><span data-stu-id="2171a-113">Key.</span></span>|
|<span data-ttu-id="2171a-114">value</span><span class="sxs-lookup"><span data-stu-id="2171a-114">value</span></span>|<span data-ttu-id="2171a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="2171a-115">Int64</span></span>|<span data-ttu-id="2171a-116">Значение</span><span class="sxs-lookup"><span data-stu-id="2171a-116">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2171a-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2171a-117">JSON representation</span></span>

<span data-ttu-id="2171a-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2171a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->