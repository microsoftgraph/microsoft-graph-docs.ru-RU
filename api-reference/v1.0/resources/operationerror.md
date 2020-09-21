---
title: Тип ресурса Оператионеррор
description: Описание ошибок в Теамсасинкоператион.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 014112d78b19ee08836139dc39d8d99b8459027b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003026"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="13e30-103">Тип ресурса Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="13e30-103">operationError resource type</span></span>

<span data-ttu-id="13e30-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13e30-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="13e30-105">Описание ошибок в [теамсасинкоператион](teamsasyncoperation.md).</span><span class="sxs-lookup"><span data-stu-id="13e30-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="13e30-106">Свойства Оператионеррор</span><span class="sxs-lookup"><span data-stu-id="13e30-106">operationError Properties</span></span>
| <span data-ttu-id="13e30-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="13e30-107">Property</span></span>     | <span data-ttu-id="13e30-108">Тип</span><span class="sxs-lookup"><span data-stu-id="13e30-108">Type</span></span>   |<span data-ttu-id="13e30-109">Описание</span><span class="sxs-lookup"><span data-stu-id="13e30-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13e30-110">code</span><span class="sxs-lookup"><span data-stu-id="13e30-110">code</span></span>|<span data-ttu-id="13e30-111">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="13e30-111">string (readonly)</span></span>|<span data-ttu-id="13e30-112">Код ошибки операции.</span><span class="sxs-lookup"><span data-stu-id="13e30-112">Operation error code.</span></span>|
|<span data-ttu-id="13e30-113">message</span><span class="sxs-lookup"><span data-stu-id="13e30-113">message</span></span>|<span data-ttu-id="13e30-114">string (только для чтения)</span><span class="sxs-lookup"><span data-stu-id="13e30-114">string (readonly)</span></span>|<span data-ttu-id="13e30-115">Сообщение об ошибке операции.</span><span class="sxs-lookup"><span data-stu-id="13e30-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13e30-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13e30-116">JSON representation</span></span>

<span data-ttu-id="13e30-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13e30-117">The following is a JSON representation of the resource.</span></span>

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

