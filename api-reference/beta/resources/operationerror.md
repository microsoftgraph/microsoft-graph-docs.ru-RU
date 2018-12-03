---
title: Тип ресурса operationError
description: Описание ошибки в teamsAsyncOperation.
ms.openlocfilehash: 0207f490328d377fedab72d2a5300baaf3645150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076988"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="42caa-103">Тип ресурса operationError</span><span class="sxs-lookup"><span data-stu-id="42caa-103">operationError resource type</span></span>

> <span data-ttu-id="42caa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="42caa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42caa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="42caa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42caa-106">Описание ошибки в [teamsAsyncOperation](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="42caa-106">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="42caa-107">operationError свойства</span><span class="sxs-lookup"><span data-stu-id="42caa-107">operationError Properties</span></span>
| <span data-ttu-id="42caa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="42caa-108">Property</span></span>     | <span data-ttu-id="42caa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="42caa-109">Type</span></span>   |<span data-ttu-id="42caa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="42caa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42caa-111">code</span><span class="sxs-lookup"><span data-stu-id="42caa-111">code</span></span>|<span data-ttu-id="42caa-112">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="42caa-112">string (readonly)</span></span>|<span data-ttu-id="42caa-113">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="42caa-113">Operation error code.</span></span>|
|<span data-ttu-id="42caa-114">message</span><span class="sxs-lookup"><span data-stu-id="42caa-114">message</span></span>|<span data-ttu-id="42caa-115">String (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="42caa-115">string (readonly)</span></span>|<span data-ttu-id="42caa-116">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="42caa-116">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="42caa-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42caa-117">JSON representation</span></span>

<span data-ttu-id="42caa-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42caa-118">The following is a JSON representation of the resource.</span></span>

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
