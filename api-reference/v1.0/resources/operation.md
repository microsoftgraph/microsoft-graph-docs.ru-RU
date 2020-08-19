---
title: Тип ресурса Operation
description: Состояние длительной операции.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c9b920bbf696e80923c1d37756d7c27e1f06ab3a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808153"
---
# <a name="operation-resource-type"></a><span data-ttu-id="d7ed9-103">Тип ресурса Operation</span><span class="sxs-lookup"><span data-stu-id="d7ed9-103">operation resource type</span></span>

<span data-ttu-id="d7ed9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7ed9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7ed9-105">Состояние длительной операции.</span><span class="sxs-lookup"><span data-stu-id="d7ed9-105">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7ed9-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d7ed9-106">JSON representation</span></span>

<span data-ttu-id="d7ed9-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7ed9-107">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="d7ed9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7ed9-108">Properties</span></span>
| <span data-ttu-id="d7ed9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7ed9-109">Property</span></span>     | <span data-ttu-id="d7ed9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7ed9-110">Type</span></span>   |<span data-ttu-id="d7ed9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7ed9-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7ed9-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ed9-112">createdDateTime</span></span>| <span data-ttu-id="d7ed9-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ed9-113">DateTimeOffset</span></span> |<span data-ttu-id="d7ed9-114">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="d7ed9-114">The start time of the operation.</span></span>|
|<span data-ttu-id="d7ed9-115">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="d7ed9-115">lastActionDateTime</span></span>| <span data-ttu-id="d7ed9-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ed9-116">DateTimeOffset</span></span> |<span data-ttu-id="d7ed9-117">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="d7ed9-117">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="d7ed9-118">status</span><span class="sxs-lookup"><span data-stu-id="d7ed9-118">status</span></span>|<span data-ttu-id="d7ed9-119">оператионстатус</span><span class="sxs-lookup"><span data-stu-id="d7ed9-119">operationStatus</span></span>|<span data-ttu-id="d7ed9-120">Текущее состояние операции: `notStarted` ,, `running` `completed` , `failed`</span><span class="sxs-lookup"><span data-stu-id="d7ed9-120">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
