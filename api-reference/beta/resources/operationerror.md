---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: d3511979cc03df496a8c12f948ddd728e3cd0c19
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998523"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="1ba5d-103">Тип ресурса Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="1ba5d-103">operationError resource type</span></span>

<span data-ttu-id="1ba5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ba5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ba5d-105">Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="1ba5d-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="1ba5d-106">Свойства Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="1ba5d-106">operationError Properties</span></span>
| <span data-ttu-id="1ba5d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ba5d-107">Property</span></span>     | <span data-ttu-id="1ba5d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1ba5d-108">Type</span></span>   |<span data-ttu-id="1ba5d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1ba5d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ba5d-110">code</span><span class="sxs-lookup"><span data-stu-id="1ba5d-110">code</span></span>|<span data-ttu-id="1ba5d-111">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="1ba5d-111">string (readonly)</span></span>|<span data-ttu-id="1ba5d-112">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="1ba5d-112">Operation error code.</span></span>|
|<span data-ttu-id="1ba5d-113">message</span><span class="sxs-lookup"><span data-stu-id="1ba5d-113">message</span></span>|<span data-ttu-id="1ba5d-114">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="1ba5d-114">string (readonly)</span></span>|<span data-ttu-id="1ba5d-115">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="1ba5d-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ba5d-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ba5d-116">JSON representation</span></span>

<span data-ttu-id="1ba5d-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ba5d-117">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


