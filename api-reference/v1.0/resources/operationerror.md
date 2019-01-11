---
title: Тип ресурса operationError
description: Описание ошибки в teamsAsyncOperation.
localization_priority: Normal
ms.openlocfilehash: 22590d7d955cf01385292d2796ad960b1c0ced41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824586"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="b57c8-103">Тип ресурса operationError</span><span class="sxs-lookup"><span data-stu-id="b57c8-103">operationError resource type</span></span>



<span data-ttu-id="b57c8-104">Описание ошибки в [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="b57c8-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="b57c8-105">operationError свойства</span><span class="sxs-lookup"><span data-stu-id="b57c8-105">operationError Properties</span></span>
| <span data-ttu-id="b57c8-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b57c8-106">Property</span></span>     | <span data-ttu-id="b57c8-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b57c8-107">Type</span></span>   |<span data-ttu-id="b57c8-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b57c8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b57c8-109">code</span><span class="sxs-lookup"><span data-stu-id="b57c8-109">code</span></span>|<span data-ttu-id="b57c8-110">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="b57c8-110">string (readonly)</span></span>|<span data-ttu-id="b57c8-111">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="b57c8-111">Operation error code.</span></span>|
|<span data-ttu-id="b57c8-112">message</span><span class="sxs-lookup"><span data-stu-id="b57c8-112">message</span></span>|<span data-ttu-id="b57c8-113">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="b57c8-113">string (readonly)</span></span>|<span data-ttu-id="b57c8-114">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="b57c8-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b57c8-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b57c8-115">JSON representation</span></span>

<span data-ttu-id="b57c8-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b57c8-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
