---
title: Тип ресурса операции
description: Состояние выполнения длительной операции.
localization_priority: Normal
ms.openlocfilehash: 4f2e2c9a6fb9eb6d26a3511c637e79822919e2f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884968"
---
# <a name="operation-resource-type"></a><span data-ttu-id="9e259-103">Тип ресурса операции</span><span class="sxs-lookup"><span data-stu-id="9e259-103">operation resource type</span></span>

<span data-ttu-id="9e259-104">Состояние выполнения длительной операции.</span><span class="sxs-lookup"><span data-stu-id="9e259-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e259-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e259-105">JSON representation</span></span>

<span data-ttu-id="9e259-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e259-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="9e259-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e259-107">Properties</span></span>
| <span data-ttu-id="9e259-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e259-108">Property</span></span>     | <span data-ttu-id="9e259-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9e259-109">Type</span></span>   |<span data-ttu-id="9e259-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9e259-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e259-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e259-111">createdDateTime</span></span>| <span data-ttu-id="9e259-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e259-112">DateTimeOffset</span></span> |<span data-ttu-id="9e259-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="9e259-113">The start time of the operation.</span></span>|
|<span data-ttu-id="9e259-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="9e259-114">lastActionDateTime</span></span>| <span data-ttu-id="9e259-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e259-115">DateTimeOffset</span></span> |<span data-ttu-id="9e259-116">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="9e259-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="9e259-117">status</span><span class="sxs-lookup"><span data-stu-id="9e259-117">status</span></span>|<span data-ttu-id="9e259-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="9e259-118">operationStatus</span></span>|<span data-ttu-id="9e259-119">Текущее состояние операции: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="9e259-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
