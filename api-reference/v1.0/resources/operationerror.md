---
title: Тип ресурса operationError
description: Описание ошибки в teamsAsyncOperation.
ms.openlocfilehash: bcd8c989c4c69336165ef1ca29e1d114d524aa9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027383"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="e1ec0-103">Тип ресурса operationError</span><span class="sxs-lookup"><span data-stu-id="e1ec0-103">operationError resource type</span></span>



<span data-ttu-id="e1ec0-104">Описание ошибки в [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="e1ec0-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="e1ec0-105">operationError свойства</span><span class="sxs-lookup"><span data-stu-id="e1ec0-105">operationError Properties</span></span>
| <span data-ttu-id="e1ec0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1ec0-106">Property</span></span>     | <span data-ttu-id="e1ec0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e1ec0-107">Type</span></span>   |<span data-ttu-id="e1ec0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e1ec0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1ec0-109">code</span><span class="sxs-lookup"><span data-stu-id="e1ec0-109">code</span></span>|<span data-ttu-id="e1ec0-110">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="e1ec0-110">string (readonly)</span></span>|<span data-ttu-id="e1ec0-111">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="e1ec0-111">Operation error code.</span></span>|
|<span data-ttu-id="e1ec0-112">message</span><span class="sxs-lookup"><span data-stu-id="e1ec0-112">message</span></span>|<span data-ttu-id="e1ec0-113">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="e1ec0-113">string (readonly)</span></span>|<span data-ttu-id="e1ec0-114">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="e1ec0-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1ec0-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1ec0-115">JSON representation</span></span>

<span data-ttu-id="e1ec0-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1ec0-116">The following is a JSON representation of the resource.</span></span>

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
