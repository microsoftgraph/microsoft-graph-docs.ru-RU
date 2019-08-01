---
title: Тип ресурса Operation
description: Состояние длительной операции.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8088d704d5a075131d5ee1b2c3b9edf75785708b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035730"
---
# <a name="operation-resource-type"></a><span data-ttu-id="6b52c-103">Тип ресурса Operation</span><span class="sxs-lookup"><span data-stu-id="6b52c-103">operation resource type</span></span>

<span data-ttu-id="6b52c-104">Состояние длительной операции.</span><span class="sxs-lookup"><span data-stu-id="6b52c-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b52c-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b52c-105">JSON representation</span></span>

<span data-ttu-id="6b52c-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b52c-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="6b52c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b52c-107">Properties</span></span>
| <span data-ttu-id="6b52c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b52c-108">Property</span></span>     | <span data-ttu-id="6b52c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6b52c-109">Type</span></span>   |<span data-ttu-id="6b52c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6b52c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b52c-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b52c-111">createdDateTime</span></span>| <span data-ttu-id="6b52c-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b52c-112">DateTimeOffset</span></span> |<span data-ttu-id="6b52c-113">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="6b52c-113">The start time of the operation.</span></span>|
|<span data-ttu-id="6b52c-114">Ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="6b52c-114">lastActionDateTime</span></span>| <span data-ttu-id="6b52c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b52c-115">DateTimeOffset</span></span> |<span data-ttu-id="6b52c-116">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="6b52c-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="6b52c-117">status</span><span class="sxs-lookup"><span data-stu-id="6b52c-117">status</span></span>|<span data-ttu-id="6b52c-118">Оператионстатус</span><span class="sxs-lookup"><span data-stu-id="6b52c-118">operationStatus</span></span>|<span data-ttu-id="6b52c-119">Текущее состояние операции: `notStarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="6b52c-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
