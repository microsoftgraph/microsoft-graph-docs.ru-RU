---
title: Тип ресурса Operation
description: Состояние длительной операции.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b7bf1daec731033bddab63ee0fa232fbf83fe3a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534143"
---
# <a name="operation-resource-type"></a><span data-ttu-id="0e3b4-103">Тип ресурса Operation</span><span class="sxs-lookup"><span data-stu-id="0e3b4-103">operation resource type</span></span>

<span data-ttu-id="0e3b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e3b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e3b4-105">Состояние длительной операции.</span><span class="sxs-lookup"><span data-stu-id="0e3b4-105">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e3b4-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0e3b4-106">JSON representation</span></span>

<span data-ttu-id="0e3b4-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0e3b4-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0e3b4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0e3b4-108">Properties</span></span>
| <span data-ttu-id="0e3b4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e3b4-109">Property</span></span>     | <span data-ttu-id="0e3b4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0e3b4-110">Type</span></span>   |<span data-ttu-id="0e3b4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0e3b4-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e3b4-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e3b4-112">createdDateTime</span></span>| <span data-ttu-id="0e3b4-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3b4-113">DateTimeOffset</span></span> |<span data-ttu-id="0e3b4-114">Время начала операции.</span><span class="sxs-lookup"><span data-stu-id="0e3b4-114">The start time of the operation.</span></span>|
|<span data-ttu-id="0e3b4-115">ластактиондатетиме</span><span class="sxs-lookup"><span data-stu-id="0e3b4-115">lastActionDateTime</span></span>| <span data-ttu-id="0e3b4-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e3b4-116">DateTimeOffset</span></span> |<span data-ttu-id="0e3b4-117">Время последнего действия операции.</span><span class="sxs-lookup"><span data-stu-id="0e3b4-117">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="0e3b4-118">status</span><span class="sxs-lookup"><span data-stu-id="0e3b4-118">status</span></span>|<span data-ttu-id="0e3b4-119">оператионстатус</span><span class="sxs-lookup"><span data-stu-id="0e3b4-119">operationStatus</span></span>|<span data-ttu-id="0e3b4-120">Текущее состояние операции: `notStarted`, `running`,, `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="0e3b4-120">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
